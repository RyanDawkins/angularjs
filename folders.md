# Angular Folder Structure

First things first is to know where does the code go? There are two popular methods to the folder structure schema. The first one I call the _type structure_ and the other is the _component structure_.

## Type Structure
The type structure centers around placing files by what _kind_ of file they are. 

Here's an example schema
```
/app
  /controllers
    loginController.js
    dashboardController.js
    gridController.js
  /services
    loginService.js
    dashboardService.js
  /directives
    gridDirective.js
  /templates
    login.html
    dashboard.html
    grid.html
  app.js
  ...
```

You can see if you want to work on the login page you have to go into the controllers folder, the services folder, and the templates folder. This is kind of messy, and it is hard to find files that you need to work on. The solution to this is the _component structure_.

## Component Structure

```
/app
  /components
    /login
      login.html
      loginController.js
      loginService.js
    /dashboard
      dashboard.html
      dashboardController.js
      dashboardService.js
  /shared
    /directives
      /grid
        grid.html
        gridDirective.js
        gridController.js
  app.js
  ...
```

You can see this is a much easier method of organizing your files. If you need to work on the login page, you just go to the login folder.

[Next: (Views)[https://github.com/RyanDawkins/angularjs/blob/master/views.md]]
