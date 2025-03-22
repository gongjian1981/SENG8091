## Requirements

### As an AI developer, you need a subsystem that can collect content from the internet
  + Create a webpage to login
    - Implement a webpage that includes a text input field named 'username' and a password field named 'password'. 
    - Add a submit button to the webpage.
  + Validate user credential
    - When When the submit button is clicked, search the database with the same username
    - if there is a record, compare its password's value with the given value, if same give credential
    - otherwise given warning message in the webpage.
  + Create a Webpage to input url
    - Implement a webpage that includes a text input field named 'url'.
    - Add a submit button to the webpage.
  + Validate URL Input
    - When the submit button is clicked, implement a validation check for the content entered in the 'url' input field.
    - The validation logic should verify that the URL starts with 'https://', contains at least one period ('.'), and one slash ('/').
    - If the URL does not meet these conditions, display a warning message on the page and cease further actions.
  + Save Valid URL Content
    - If the URL is valid, write a function to save the content retrieved from the URL to a database.
  + Create a Web Scraping Program
    - Develop a function that can scrape content from the URL provided if it has passed the validation check.
    - Ensure the scraper can handle and parse the content appropriately for storing in the database.
  + Develop a Method to Load All URLs
    - Implement a method to retrieve all previously saved URLs from the database.
    - Ensure this method efficiently handles a large volume of URLs and includes necessary error handling mechanisms.
  + Scrape and Store Content from Embedded URLs
    - Extend your web scraping program to not only scrape the main URL's content but also identify and scrape content from other URLs embedded within the page.
    - For each discovered embedded URL, repeat the previous validation and storage process.
    - Ensure the program can avoid repeatedly scraping the same URL and correctly handle circular references.

### As an AI developer, you need a subsystem that can have categorized training questions that are separate from the answers
  + Design Data Model for Categorization
    - Define the database schema for separating questions and answers in the training data.
    - Content table should have id(int), content(str), type(int) (which 0 stands for question, 1 for answer), category_id(int)
    - Category table should have id(int), name(str)
  + Create a Webpage for Data Input
    - Develop a webpage with a div field which display training data.
    - A set of radio buttons labeled "Question" and "Answer" to categorize the input as either a question or an answer.
    - A submit button to send the data to the server.
  + Create a API to receive question/answer data and save to the database
    - Implement a method which accept 2 parameters with content as type 'string' and type as type 'int'
    - save the content and type to the database
  + Create a Webpage for Categorizing
    - A list of texts each with a checkbox in front of them.
    - A select with different categories as its options.
    - A submit button
  + Create a API to receive category data and save to the database
    - Implement a method which accept 2 parameters with content_id as type 'int' and category_id as type 'int'
    - update the category_id to the content with the corresponding id to the database
### As an AI developer, you need a AI system that can using these filtered contents to train and provide result based on algorithm
  + Implement Bias Check on Data Submission
    - Integrate a bias detection library within the form submission handling process.
    - Run a bias check when data is submitted and categorize the bias level.
  + Create a Webpage for All the data
    - Develop a webpage that displays the list of bias content
    - The content can click to see its detail
    - Provide 1 'Accept' button for the user to accept the bias assessment,
    - Provide 1 'Dispute' button for the user to dispute it.