## Unit Tests:

A unit test refers to an individual component in the code.
The so-called unit can be anything we use in the code. In most
case scenarios we a unit would be a class, but it could also be a function
or a group of functions related to the same context. Unit tests make sure that a single class/function implements all methods properly with automated unit tests.
Unit tests are rarely performed manually. That coverage is often done trough 
integration testing.

### Code example:

Let's take the following class of DemoController. This will be our unit.

```js
// demo.controller.js
export class DemoController {
  public getParam(param = 0) {
    return param;
  }
}

// demo.controller.test.js
import { DemoController } from './demo.controller';

describe('DemoController', () => {
  let controller: DemoController;

  beforeEach(async () => {
    controller = new DemoController();
  });

  it('should get 0', () => {
    expect(controller.getParam()).toBe(5);
  });
});

```

When defining unit tests we usually try to cover as many cases as we can. 
Here we can cover:
- Is the method callable
- Does it by default return 0
- Does it return the value we pass it.
- etc

A simple function with only one line can have multiple tests. The amount of code we test here is 
referred to as coverage and many tools help us visually display the code we covered. 

In TDD (Test Driven Development) we first write the unit tests and then implement the units based on those tests.

## White Box Tests:

In programming when you are working with something you know the internal parts of it is usually called `white XYZ`. For example when we use a library with npm that is something of a `black box` to us as we do not know the code. While the code we write is the `white code` so to speak of. 

When testing a part of an app white box testing would be that the tester has a good understanding of how the code works and all cases covered by it.

### Code example

```js
function log(message, type) {
  switch(type) {
    case 'info':
      console.info(message);
      break;
    case 'error':
      console.error(message);
      break;
    default:
      console.log(message);
  }
}
```

Here we have a function that logs a message using the appropriate method. Knowing the logic behind the method we can:

>a) Focus our test cases to cover what is implemented

>b) Notice missing cases and functionalities we can report

White box test helps us easier define test cases as we know what we should test based on the code, but does not help us too much with cases that are missing in the function.

It is pretty easy now to define cases here where we check that all 3 switch cases are hit based on passed arguments.

## Black Box Tests

Black box testing gives us very little information on how a feature works. We only know what it does.

On a login form, we have a `password` and `username` field and submit button. Semantically we know what the form does, but not really how it is implemented behind. Is the password encrypted in the database, do we use a third-party service to authorize the user, is there a not robot mechanism present. 

We do not know, and that is what is great about black-box tests. We know what the client wants and we have a form in front of us. When having code in front of us we often limit ourselves to cover what we see there. Now here we can get creative. We do not care about the code. We care about the requirements.

There is no concrete code example here. All we have is:
 
- Our input
- The black box app
- The output of the app

Now, all we have to do is structure our cases:

> When I enter a valid username and password it should log me in

> When I enter an invalid username and password it should let me know

> When I input `xyz` the app should output `abc`

> ...

Unit tests are something more suited for white box testing while integration tests cover it more in a black-box way.


## Gray Box Tests

This is a hybrid method that combines `black box` and `white box` tests. The simplest approach to it would be that tester has access to the source code, but does not structure the cases based on it. In black-box tests, we structure our tests by what we expect and in gray-box, we expand on that by going into the code after we performed most black-box tests.

Another method would be having a diagram of flow for our feature. We do now know the internal behaviors of the code, but we have a pretty certain idea of how it works. 

Since this is a combination of two test methodologies using both approaches would also be a type of gray box testing.

### Code Example

Gray box testing is testing with limited knowledge of the application. An example of gray box testing is functional testing. In the second image, we can test a calculator created with HTML code and make changes if a button doesn’t work and we can change the backend code (white box testing) and features with the frontend code (black-box testing)

![](https://miro.medium.com/max/700/1*UsZ207XnbgSM7ZE-565bOA.png)


![](https://miro.medium.com/max/700/1*VhQ4o_We4lXENHztj-IDZg.png)