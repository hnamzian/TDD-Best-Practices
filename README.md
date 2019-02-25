# Why using Automated Testing

## Benefits of TDD

1- Test the code frequently in less time

2- Catch bugs before deploying

3- Deploy with confidence

4- Refactoring the code with confidence

5- Focus on the quality of methods

## Types of tests

1- Unit Test: Tests a unit of the application without its **external dependencies** such as databases, web services, etc. It's cheap to write and executed very fast. As the dependencies are not tested it wont give a lot of confidence.

2- Integration Test: Tests components with their external dependencies. Traditionally it takes a few units or classes of the application and tests the behaviour as whole. It gives more confidence in the price taking more time.

3- End-to-End Test: Drives an application through its UI using special tools such as Selenium to record test scenariosa and then play it back and test the application. It takes too long but gives the greatest confidence. A small changes in the UI will breake tests.

## Best Practice

- Most of the automated tests should be done in the category of unit test as it's easy to write and executed quickly.
- Unit tests are great to test the logic, like conditional statement and loops. For methods with complex logic and calcualtions unit tests are ideal.
- Favour unit tests over integration tests and e2e tests as they are easy to write, executed fast, accurate and shows exactly the point of failure.
- Write a bunch of tests using integration tests which tests the intrgration of application with external dependencies. It provides many advantage of e2e test without the complexities of dealing with UI.
- Write very few e2e tests only for key functions of application.

## Testing Frameworks

- Jasmine
- Mocha: Most popular testing framework on npm. It lacks some certain features and packages like **chai** and **Sinon** needed to be used alongside.
- **Jest**: Newer framework Facebook use it for its react projects. It's actually a wrapper around Jasmine with built-in code coverage tool.
  
Tools and frameworks don't really matter. Focus on the **fundamentals** of writing tests.