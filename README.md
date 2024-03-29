
# RESTful - A simple Spring MVC todo list with RESTful api development

## About This Project

The project was created with the purpose of providing a better understanding of RESTful API development. Initially, a simple todo list project was built using the SpringBoot framework. This project included a Controller class that implemented all CRUD operations (Create, Read, Update, and Delete)

![demo](https://github.com/han-ziqi/RESTful/raw/master/demo/CRUD%20demo.png)
This is a demo for CRUD html interface

The next step in the project involved transforming the Controller class to adhere to RESTful architecture principles. This involved designing RESTful endpoints that allowed for efficient handling of server requests and responses, improving the user experience.

`Java` was the primary language utilized throughout the project, with additional knowledge of `Spring MVC` and  `Ajax`.In addition, the use of software `Postman` to test the Requests. 

![postman](https://github.com/han-ziqi/RESTful/raw/master/demo/Postman.png)
This is the Postman software to test POST/PUT

## Curriculum design
This project can be used as a curriculum design for, for example, **three hours to learn RESTful style software design**.

### Course Overview:

This course is designed for developers who want to learn how to create a RESTful API using SpringBoot framework. The course will cover the basics of creating a simple Todo list project and adapting its main controller class to use RESTful style.

### Course Outline:

#### Traditional vs. front and back-end separation
The traditional development model
Front-end write static html pages to the back-end development, the back-end html into a template, and then use the template engine to set the template, such as jsp, freemarker, etc. Back-end personnel in the development process, if you find a problem with the page, to return to the front-end to modify, the front-end and then to the back-end, until the function is achieved.

Problems: serious coupling between front-end and back-end
1. when the front-end needs to change the bug debugging, you need to install a full set of back-end development tools in the current computer, start the back-end program.
2. It also requires back-end personnel to know html, js and other front-end languages.
3. The front-end page will also embed a lot of back-end code
4. Once the back-end has changed a set of language, the front-end also needs to be redeveloped
5. communication costs, debugging costs, front-end and back-end development progress affect each other, thus greatly reducing development efficiency

#### Separation of front and back ends
The separation of front and back ends is not just a development model, it is also an architectural model for web applications. In the development phase, the front and back-end people agree on the data interaction interface and can develop and test in parallel.
The front end can be mock tested alone, while the back end can be tested using interface testing tools such as postman. Finally, functional testing can be done in conjunction with the testing.

Advantages:
1. Clear responsibility for the front and back end, with the back end focusing on the data and the front end on the visuals.
2. No need to wait for each other's development work to finish, improving development efficiency.
3. Can cope with complex and changing front-end requirements.
4. Enhances code maintainability

- Introduction to RESTful APIs
1. What is API?
  An API (Application Programming Interface) is a number of predefined functions, or conventions for interfacing different components of a software system. The purpose is to provide applications and developers with the ability to access a set of routines based on a piece of software or hardware, without having to access the original code or understand the details of the internal workings.
2. What is a RESTful API?
  A RESTful API is a type of web service that uses HTTP requests to access and manipulate resources over the internet, based on the principles of the HTTP protocol. Resources are identified by a unique URL, and different HTTP methods such as GET, POST, PUT, DELETE, etc. are used to perform different operations on the resource. RESTful APIs typically use a stateless client-server architecture and are flexible, scalable, and easy to understand and implement, making them popular for building a wide range of applications.

- Overview of the course

1. Setting up the Development Environment
   1. Installing Java and SpringBoot
   2. Creating a new SpringBoot project
   3. Setting up the project structure
2. Building a Todo List Project
   1. Creating the Todo model class
   2. Creating the Todo repository class
   3. Creating the Todo service class
   4. Creating the Todo controller class
   5. Testing the Todo controller class
3. Adapting the Controller Class to Use RESTful Style
   1. Overview of RESTful architecture
   2. Creating RESTful endpoints for Todo resources
   3. Implementing CRUD operations using RESTful endpoints
   4. Testing the RESTful endpoints using Postman software

Recap of the course

1. Request path
   Determine the specific operation resources, combined with the needs, you can add the path prefix and suffix as appropriate, or use the parameter path way
2. Request method
   According to the actual function of the interface, find the appropriate method for the CRUD of the resource
   1. Resources from nothing: POST
   2. Resources from yes to no: DELETE
   3. Resource from state A to state B: PUT
   4. Resource state does not change: GET

3. Request parameters
   Parameters are passed in as required according to the function of the interface implementation

3. Request response
   According to the interface implementation, the client calls the requirements to determine the specific return value, it is recommended to use JSON format.


