# Day 1 - Inception

### Ques 1 -> What is Emmet?

Ans:

- Emmet is a set of plug-ins for text editors that allow for high-speed coding and editing in HTML, XML, XSLT, and other structured code formats via content assist.
- Emmet is primarily independent from any text editor, as the engine works directly with text rather than with any particular software.
- Emmet uses a specific syntax in order to expand small snippets of code, similar to CSS selectors, into full-fledged HTML code.

E.g. p>h1 gives :

```bash
<p>
  <h1></h1>
</p>
```

### Ques 2 -> Difference between a Library and Framework?

Ans:

- A library is a collection of reusable code that allow a user to use in programs or applications to perform specific tasks. Its example are JQuery , React JS , etc.
- A framework is a more comprehensive set of tools that provides a structure for developing applications. Its example are AngularJS , Spring , NodeJS , etc.

- A framework inverts the control of the program. It tells the developer what they need. A library doesn’t. The programmer calls the library where and when they need it.
- Consider an example that Library is an your home and framwork is an your school. when there is less number of rule that is library. when there is more number of rules that is framwork. library is simpal collection of code some functions or Dom objected model are packed together it use over and over, You only call your library. framwork simply call your code and further your code calls to library maybe. example: jQuary is library where as Django is Framwork
- A library is like going to Ikea. You already have a home, but you need a bit of help with furniture. You don’t feel like making your own table from scratch. Ikea allows you to pick and choose different things to go in your home. You are in control. A framework, on the other hand, is like building a model home. You have a set of blueprints and a few limited choices when it comes to architecture and design. Ultimately, the contractor and blueprint are in control. And they will let you know when and where you can provide your input.

### Ques 3 -> What is CDN? Why do we use it?

Ans:
A content delivery network (CDN) is a distributed system of servers that delivers web content to users based on their geographic location. CDNs are used to improve the performance and availability of websites, applications, and other online content by serving it from a location that is closer to the user.

CDNs work by caching static content, such as images, videos, and stylesheets, on a network of servers that are located at strategic points around the globe. When a user accesses a website that is using a CDN, the CDN redirects the request to the server that is nearest to the user's location, which reduces the time it takes for the content to be delivered.

There are several benefits to using a CDN:

- Improved performance: CDNs can significantly improve the loading speed of a website or application by reducing the distance that the content has to travel. This is especially important for users who are located far from the origin server, as the content will be delivered to them faster.

- Greater scalability: CDNs can handle large spikes in traffic without experiencing performance issues, as the content is distributed across multiple servers. This makes them ideal for websites or applications that experience a lot of traffic or have a global user base.

- Enhanced security: CDNs can help protect against DDoS attacks and other security threats by distributing the traffic across multiple servers and providing additional layers of protection.

- Greater reliability: CDNs can help ensure that a website or application is always available by providing multiple copies of the content on different servers. If one server goes down, the CDN can redirect the traffic to another server.

In summary, CDNs are used to improve the performance, scalability, security, and reliability of websites and applications by delivering content from a location that is closer to the user.

### Ques 4 -> Why is React known as React?

Ans:

- React was developed for applications (Facebook) that have constantly changing data.
  Since React is a front-end framework or the “View” in MVC, this means that as the user clicks around and changes the app's data,
  the view should “react” or change with those user events.

  or

React is known as React because it was developed and is maintained by Facebook, and the name "React" is short for "Reactive".

React is a JavaScript library for building user interfaces that was created by Facebook engineer Jordan Walke in 2011. It was initially developed to solve the problem of efficiently rendering large lists of data, such as those found in social media feeds.

The key idea behind React is that a user interface should be a declarative representation of the data it displays. In other words, the user interface should "react" to changes in the data by updating itself automatically, rather than requiring the developer to manually update it. This makes it easier to build and maintain complex user interfaces, as the developer only has to worry about the data, rather than the details of how it is displayed.

React has become widely popular due to its simplicity, flexibility, and performance. It is used by many companies and organizations, including Facebook, Airbnb, Netflix, and the New York Times, to build complex and scalable user interfaces.

In summary, React is known as React because it was developed by Facebook and is a reactive library for building user interfaces.

### Ques 5 -> What is crossorigin in script tag?

Ans:
The crossorigin attribute in a script tag specifies the CORS (Cross-Origin Resource Sharing) policy for the script. It is used to indicate whether the script should be treated as a "same-origin" script or a "cross-origin" script.

A "same-origin" script is a script that is loaded from the same origin (protocol, domain, and port) as the webpage that includes it. A "cross-origin" script is a script that is loaded from a different origin than the webpage that includes it.

The crossorigin attribute can have one of two values: anonymous or use-credentials.

If the crossorigin attribute is set to anonymous, the script will be treated as a "cross-origin" script, but no credentials (such as cookies or HTTP authentication) will be sent with the request. This is useful for scripts that do not require authentication or that are hosted on a CDN (Content Delivery Network).

If the crossorigin attribute is set to use-credentials, the script will be treated as a "cross-origin" script, and credentials will be sent with the request. This is useful for scripts that require authentication or that are hosted on a private server.

Here is an example of a script tag with the crossorigin attribute set to anonymous:

```
<script src="https://example.com/script.js" crossorigin="anonymous"></script>
```

In this example, the script will be treated as a "cross-origin" script and will be loaded from the origin https://example.com, but no credentials will be sent with the request.

The crossorigin attribute is used to ensure that the browser handles cross-origin requests for scripts in a secure and consistent manner. It is particularly important when loading scripts from a CDN, as it allows the CDN to properly handle requests from different origins.

### Ques 6 -> What is diference between React and ReactDOM?

Ans:

- React library is responsible for creating views

- ReactDOM library is responsible to actually render UI in the browser.

### Ques 7 -> What is difference between react.development.js and react.production.js files via CDN?

Ans:

The react.development.js and react.production.js files are different versions of the React library that are optimized for different use cases.

The react.development.js file is intended for use during development, and includes extra debugging information and helpful warning messages that can make it easier to identify and fix problems in your code. It is also not minified, which means that the code is easier to read and debug, but it is larger in size than the react.production.js file.

On the other hand, the react.production.js file is intended for use in a production environment, where the focus is on optimizing the performance of the application. It is minified, which means that the code has been compressed to make it as small as possible, and it does not include the extra debugging information and warning messages that are present in the development version.

It's generally recommended to use the production version of React in a live application, as it will be faster and more efficient than the development version. However, during development, you may find it helpful to use the development version so that you can see any warning messages or other debugging information that may be helpful in identifying and fixing issues in your code.

### Ques 8 -> What is async and defer?

Ans:

- async will fetch the js file in parallel while parsing HTML and once the file is fetched the HTML parsing is paused and the js scripts are executed with the guarantee of the order of execution and once it executed the HTML parsing is resumed.

- defer will fetch the js file in parallel while parsing the HTML and once the HTML is parsed completely then the scripts are executed in the given order.
