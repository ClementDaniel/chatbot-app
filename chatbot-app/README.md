# Build a Food Order Chatbot using AWS 

| Amazon Lex     | Provides the chatbot functionality, allowing users to interact with th system via voice or text. Handles natural language processing to understand user input and respond accordingly                             |
| AWS Lambda     | Executes backend logic. It uses the built-in integration capability with Lex to process inputs from Lex (e.g. parsing user orders, validating data, handling business and fulfilment logic) and returns responses |
| Amazon S3      | Hosts the static assets (such as HTML, CSS and JavaScript files) for the frontend webpage where the Lex chatbot is embedded                                                                                       |
| AWS Cloudfront | Distributes the frontend webpage content via a Content Delivery Network (CDN), ensuring fast and secure delivery of the website globally                                                                          |
| Amazon Cognito | Handles user authentication for the frontend, providing secure access to the web interface for users interacting with the chatbot                                                                                 |

## Features:
This chatbot allows you to order and customize a burger with the following characteristics:
- Order a Burger from 3 different Franchises
- Each Franchise has 3 unique toppings
- Order a Burger in 3 different sizes
- Choose from a selection of sides and drinks
- The Chatbot enforces the above logic (i.e. if you select an incorrect topping from a respective Franchise, the bot will automatically prompt you with an error message)

