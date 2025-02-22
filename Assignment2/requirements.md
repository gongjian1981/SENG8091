## Requirements
### Functional Requirements
- As an AI developer, you need a subsystem that can collect content from the internet
  + the system should save urls entered by users.
  + the system should get content on the internet of the urls saved.
  + the system should give the content scraped to the data abstraction system.
- As an AI developer, you need a subsystem that can filter these contents
  + the system should receive content and save to the system.
  + the system should have categorized training questions that are separate from the answers
  + the system should know that the training data is “balanced”
- As an AI developer, you need a AI system that can using these filtered contents to train and provide result based on algorithm
  + the system should provide a entrance for administrator to input data.
  + the system should be able to analyse the data based on the model.
  + the system should generate answer to the question user input.
### Non-Functional Requirements
- for web scraping, it needs to be automated and keep running
  + the system should be reliability, it needs to be working 7x24.
  + the system should be fast, it should take a short time to scraping a web page.
  + the system should be able to run simultaneously, support multi threads to work at the same time.
- for data abstraction, it also needs to be automated and provide correct data
  + the system should be able to save a large amount of data.
  + the system should be able to enlarge the storage easily.
  + the system should comply with data protection regulations.
- for AI System, it needs to be easy for user to use and easy to train
  + the system should be security so that only administrator can train the data.
  + the system should be user-friendly, all users should be interact with the system.
  + the system should be easy to update.