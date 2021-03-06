[![Build Status](https://travis-ci.org/judeinno/StackOverFlow-lite-Challeng-3.svg?branch=Challenge3)](https://travis-ci.org/judeinno/StackOverFlow-lite-Challeng-3)


# StackOverFlow-lite

This is a question answer app that allows users to ask questions and as well give replys.
it also allows a users to vote for a question and also comment on it

# Main requirements include:
> 1. [git](https://git-scm.com/)
> 2. [python](https://docs.python.org/) 
> 3. [pip](https://pypi.python.org/pypi/pip) 
> 4. [virtualenv](https://virtualenv.pypa.io/en/stable/)
> 4. [Postgres](https://www.postgresql.org/) 

# Getting Started
1. Clone the project

`git clone https://github.com/judeinno/StackOverFlow-lite.git`

2. Create a virtual environment using `virtualenv` and activate it.

`virtualenv venv`
`venv\Scripts\Activate`

3. Install packages using `pip install -r requirements.txt`

4. Run the app by running `run.py`

`python run.py`


# Project Link
__Interface__
The link to the pages hosted on gh-pages is:
 https://judeinno.github.io/StackOverFlow-lite/templetes/index.html

The link to git hub feature branch with the code is:
https://github.com/judeinno/StackOverFlow-lite/tree/feat/UI-templetes

__API endpoints__

The link to the git hub branch with the code is:
https://github.com/judeinno/StackOverFlow-lite/tree/API


 # Features
__interface__
- Users can create an account and log in.
- The users can ask questions on home page.
- User can view recently asked questions.
- User can vote up and vote down an answer
- User can comment on an answer

__API endpoints__

| End Point                                           | Verb |Use                                   |
| ----------------------------------------------------|------|--------------------------------------|
|`/api/v1/`                                           |GET   |API prefix                            |
|`/api/v1/questions`                                  |GET   |Gets a list of Questions              |
|`/api/v1/questions`                                  |POST  |Post a question                       |
|`/api/v1/questions/<int:qn_id>`                      |GET   |Gets a Question resource of a given ID|
|`/api/v1.0/questions/<int:qn_id>/answers`            |POST  |Adds a an answer to a question        |
|`/api/v1.0/questions/<int:qn_id>        `            |DELETE|Delete  a question                    |
|`/api/v1.0/questions/<int:qn_id>/answers`            |POST  |Adds a an answer to a question        |
|`/api/v1.0/questions/<int:qn_id>/answers/<int:ans_id>` |PUT  |Modify an answer to a question        |

# How  the arguments are to be passed in postman
  * Users register Endpoint takes the following data.  
  ` {
	"username":"username",
	"email":"email",
	"password":"password"
	`
   * Users register Endpoint takes the data as follows.  
  ` {
	"username":"username",
	"password":"password"
	`
    `    
   * Users Question json data Endpoint takes the data follows.  
   `
   {
      "Question": "string"
    }
    `

   * Users Answer json data Endpoint takes the data follows.  
   `
   {
      "Answer": "string"
    }
    `

# Built With
__interface__
- HTML5
- CSS

__API endpoints__
- Python 3
- Flask
- Flask restful

# Prerequisites
- HTML 5
- Internet

# Authors
Atuhaire Jude Innocent

# Licensing

The app is opensource hence free to all users

- Web browser with support for HTML5
- Internet connection