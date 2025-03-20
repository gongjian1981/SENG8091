## Challenge 1
to have categorized training questions that are separate from the answers

### Functional Requirements
- as an AI developer, you need the system be able to process data from various sources and formats
  + the system should be able to analysis basic structure of a webpage.
  + the system should be able to abstract content from the webpage based on its structure
  + the system should be able to jump over those contents cannot read and save to the database
- as an AI developer, you need to separate questions from answers
  + the system shoule be able to tell which sentences are questions
  + the system shoule be able to tell which sentences are answers
  + the system shoule be able to save sentences and answers in different place.
- as an AI developer, you need to have the questions categorized
  + the system shoule be able to create categories.
  + the system shoule be able to tell a question belong to which category.
  + the system shoule be able to save the question to its corresponding category.

### Assumptions
- the content is multilanguages
- a question without answer is useless
- a question that can be categoried is still needed
### Validation
- Do the system need to support multilanguages
- Do all the questions need answers
- Do all the questions that can be categoried need to be categoried later

### Tasks
- build system that support main languages
- build system that only deal questions with answers
- build system that support categorize those uncategoriez question