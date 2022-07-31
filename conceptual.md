### Conceptual Exercise

Answer the following questions below:

- What is a JWT?

# Json web token make request for username/password to login route and keeps track of the request. Server Authenticates and puts user into session

- What is the signature portion of the JWT?  What does it do?

# The signature is authentic to the token of the user. It combines the Header (metadata about the token) as well as the payload(data to be stored in token)

- If a JWT is intercepted, can the attacker see what's inside the payload?

# The attacker would get the header and payload but the signature is unique to verify the origin or to identify the sender

- How can you implement authentication with a JWT?  Describe how it works at a high level.

  # Client send a login request with username and password to server
  # Server receive the username and password,   authenticate the user
  # If authentication is successful, then the server  creates a JWT token called accessToken that  stores user public info and sends it back to the   client.
  # Client receives the accessToken, from now on,   client sends any request to server, client just   attach the accessToken with request
  # Server receives a request, authenticates the JWT  token, and continues processing the request, and   then returns the result to the client


- Compare and contrast unit, integration and end-to-end tests.

  # Unit Test are code that effeciently test code through isolated small pieces. End to End takes the entire application and makes it a comprehensive in a real-world scenerio. Integration is in the minidle of the two tests and tests what parts work together.

- What is a mock? What are some things you would mock?

  # Mock is primarily used for unit testing. An object under test may have dependencies on other complex objects. To mock, you would have to isolate and replace the other objects that simulate the behavior

- What is continuous integration?

  # Continous integration is the practice of merging in small code changes frequently. The goal is to build better software by developing and testing in small increments.

- What is an environment variable and what are they used for?

  #Enviroment variables all your app to behave differently based on the enviroment you want them to run in. Whenever you want to do configurations you use enviroment variables.

- What is TDD? What are some benefits and drawbacks?

  # TDD (Test Driven Development), is writing the code with testing first in mind. It could help with thinking of this as to help with structure of the code. TDD is helpful for helping with getting better at testing. The giffest con is it can slows development upfront.

- What is the value of using JSONSchema for validation?

 # JsonSchema is meant so user data can fail fast before bad data gets to your database. It can reduce amount of code for processing and validating data. To get a valiation system that is easy to setyp and maintain.

- What are some ways to decide which code to test?

# Dont get attached to coverage percentages. Instead of testing db, test API.

- What does `RETURNING` do in SQL? When would you use it?
  # RETURNING is used for Insert/Update/Delete, this is to return the data from the ones that are mentioned.

- What are some differences between Web Sockets and HTTP?

  # Unlike HTTP, where you have to constantly request updates, with websockets, updates are sent immediately when they are available. WebSockets keeps a single, persistent connection open while eliminating latency problems that arise with HTTP request/response-based methods.



- Did you prefer using Flask over Express? Why or why not (there is no right
  answer here --- we want to see how you think about technology)?


  # For right now, I am liking express. It's not less work than flask, but it feels simple and able to see where the mistakes you've made. 