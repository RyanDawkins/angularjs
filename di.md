# Dependency Injection

Dependency Injection is a creational design pattern. The idea in angular is we have all of these singleton objects and we inject them into what asks for them.

The rational around creating these dependencies comes from several ideas. First **seperation of concerns**, this promotes allowing our controllers to be skinny, and prevents a lot of I/O related code from being in places they shouldn't. Second, by design it allows us to mock the dependencies so that we can test these things without testing other code.

[Next: Angular Folder Structure](https://github.com/RyanDawkins/angularjs/edit/master/folders.md)
