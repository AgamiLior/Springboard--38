### Conceptual Exercise

Answer the following questions below:

- What is a JWT?
    -  Jason Web Tokern, It is an encrypted token generated after authentication to make response between the user and the backend of the app.

- What is the signature portion of the JWT?  What does it do?
    - JWT usualy contains three parts:
        1. Header
        2. Payload
        3. cryptographig signature.
        The signature is used verify that the user who send this req is valid.
        
- If a JWT is intercepted, can the attacker see what's inside the payload?
    - Yes, if JWT is intercepted the attacker can use decode to see what is inside the payload.
    
- How can you implement authentication with a JWT?  Describe how it works at a high level.

    - Client send a login request with username and password to server,The server receive the username and
    password, authenticate the user.
    If authentication is successful, then the server creates a JWT token that stores user public info and sends
    it back to the client. From now on, client sends any request to server, client just attach the accessToken
    with request.
    Server receives a request, authenticates the JWT token, and continues processing the request, and then
    returns the result to the client.
    
- Compare and contrast unit, integration and end-to-end tests.
    -   Unit testing means testing individual modules of an application in isolation (without any interaction
    with dependencies) to confirm that the code is doing things right. Integration testing means checking if
    different modules are working fine when combined together as a group.
    What is E2E Integration testing?
    End-to-end testing is a technique that tests the entire software product from beginning to end to ensure the
    application flow behaves as expected.
    
- What is a mock? What are some things you would mock?
    - Mocking is a very popular approach for handling dependencies while unit testing.
    
- What is continuous integration?
    - DevOps software development practice where developers regularly merge their code changes into a central
    repository, after which automated builds and tests are run.
    
- What is an environment variable and what are they used for?
    - Enviroment variable exsists to declare the platform of which we run our code, either normal or test.
    It lets the program understand which files to use, and which user settings to use.
    
- What is TDD? What are some benefits and drawbacks?
    - Test Driven Development the pros and cons are:
        * pros:  
            you only write code that's needed
            more modular design
            easier to maintain
            easier to refactor
            high test coverage
            tests document the code
            less debugging
        * cons:
            slow process
            everybody got to do it.
            
- What is the value of using JSONSchema for validation?
    - It provides the language for the human and the machine to understand the stracture of instance data. 
- What are some ways to decide which code to test?

- What does `RETURNING` do in SQL? When would you use it?
    -  Allows you to retrieve values of columns that were modified by an insert, delete or update.
    
- What are some differences between Web Sockets and HTTP?
    - Unlike HTTP, where you have to constantly request updates, with websockets, updates are sent immediately when they are available. WebSockets keeps a single, persistent connection open while eliminating latency problems that arise with HTTP request/response-based methods.
    
- Did you prefer using Flask over Express? Why or why not (there is no right
  answer here --- we want to see how you think about technology)?
    - I prefred using Flask as it was easier to understand, The level of complicity of using SQL in express is more demanding.
