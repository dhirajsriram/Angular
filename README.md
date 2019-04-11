# Angular 

Angular is a platform that makes it easy to build applications with the web. Angular combines declarative templates, dependency injection, end to end tooling, and integrated best practices to solve development challenges. Angular empowers developers to build applications that live on the web, mobile, or the desktop.

## Prerequisites

### Node.js

Angular requires Node.js version 8.x or 10.x.

### npm package manager

Angular, the Angular CLI, and Angular apps depend on features and functionality provided by libraries that are available as npm packages. 

## Architecture

The following screenshot shows the anatomy of an Angular 2 application. Each application consists of

- Components

- Modules 

- Services and dependency injection

- Routing

### Components

Each component is a logical boundary of functionality for the application. Following is the anatomy of a Component. A component consists of −

- Class − This is like a C++ or Java class which consists of properties and methods.

- Metadata − This is used to decorate the class and extend the functionality of the class.

- Template − This is used to define the HTML view which is displayed in the application.

<p align="center">
<img src="https://www.tutorialspoint.com/angular2/images/componet.jpg">
</p>

Following is an example of a component.

``` ts
import { Component } from '@angular/core';

@Component ({ 
   selector: 'my-app', 
   templateUrl: 'app/app.component.html' 
}) 

export class AppComponent { 
   appTitle: string = 'Welcome';
} 
```

### Modules

An angular module can be looked at as the inception point for any angular application. The root angular module is named *appmodule* by default. A module provides a bootstrap mechanism for how an angular appication must run.

Like JavaScript modules, *NgModules* (angular module) can import functionality from other *NgModules*, and allow their own functionality to be exported and used by other *NgModules*. For example, to use the router service in your app, you import the Router *NgModule*.

Organizing your code into distinct functional modules helps in managing development of complex applications, and in designing for reusability. In addition, this technique lets you take advantage of lazy-loading—that is, loading modules on demand—to minimize the amount of code that needs to be loaded at startup.

### Services

You need to have layered services, which are used to share the functionality across components. Services provide components with data and functionality which can be shared across 

<p align="center">
<img src="https://www.tutorialspoint.com/angular2/images/anatomy.jpg">
   </p>

### Routing

Routing is what makes angular a full fledged SPA framework. With routing a user will be able to iteract with the components and navigate to the component in demand, Router is modeled on the familiar browser navigation conventions:

- Enter a URL in the address bar and the browser navigates to a corresponding page.

- Click links on the page and the browser navigates to a new page.

- Click the browser's back and forward buttons and the browser navigates backward and forward through the history of pages you've seen.

The router maps URL-like paths to views instead of pages. When a user performs an action, such as clicking a link, that would load a new page in the browser, the router intercepts the browser's behavior, and shows or hides view hierarchies.

The router interprets a link URL according to your app's view navigation rules and data state. You can navigate to new views when the user clicks a button or selects from a drop box, or in response to some other stimulus from any source. The router logs activity in the browser's history, so the back and forward browser buttons work as well.

### Architecture

Following would be a good representation of how the induvidual sturctures of Angular interact with each other

<p align="center">
<img src="https://angular.io/generated/images/guide/architecture/overview2.png">
</p>

## Features

### Cross Platform

#### Desktop

Create desktop-installed apps across Mac, Windows, and Linux using the same Angular methods you've learned for the web plus the ability to access native OS APIs.

#### Progressive web apps

Use modern web platform capabilities to deliver app-like experiences. High performance, offline, and zero-step installation.

#### Native

Build native mobile apps with strategies from Cordova, Ionic, or NativeScript.

### Speed and performance

#### Code Generation

Angular turns your templates into code that's highly optimized for today's JavaScript virtual machines, giving you all the benefits of hand-written code with the productivity of a framework.

#### Universal

Serve the first view of your application on Node.js®, .NET, PHP, and other servers for near-instant rendering in just HTML and CSS. Also paves the way for sites that optimize for SEO.

#### Code Splitting

Angular apps load quickly with the new Component Router, which delivers automatic code-splitting so users only load code required to render the view they request.

### Productivity

#### Templates

Quickly create UI views with simple and powerful template syntax.

#### Angular CLI

Command line tools: start building fast, add components and tests, then instantly deploy.

### Development

#### Animation

Create high-performance, complex choreographies and animation timelines with very little code through Angular's intuitive API.

#### Accessibility

Create accessible applications with ARIA-enabled components, developer guides, and built-in a11y test infrastructure.




