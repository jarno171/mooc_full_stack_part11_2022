# Exercise 1

## Language: Python

Python is a popular language, used for many different purposes (data-science, machine learning, for building websites and software).

### Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked?

Because Python is a popular programming language, there are many VS Code extensions for static python code analysis (for example, "Python" by Microsoft, "Lightrun" or "Flake8"). Programmatically Python can be linted with ex. Pylint, which can be used in Github actions.

There are many Python testing frameworks and libraries depending on the purpose of the testing ("PyTest", "Robot Framework" etc.)

Python programs can be packaged and released with, for example "Poetry", which is a Python packaging and dependency management.

### What alternatives are there to set up the CI besides Jenkins and GitHub Actions?

One obvious alternative to GitHub is Gitlab, which resembles Gitlab, but there are some differences. Gitlab is most often used with third party CI-programs like Jenkins, and they advocate for different kind of workflows by default (Github advocates merging new changes with main-branch, while Gitlab advises to use multiple stable branches, https://www.zdnet.com/article/github-vs-gitlab-the-key-differences/).

There are other frameworks too, like "Buildbot" and "CircleCI", to name a few.

### Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?

It depends on the scale of the project, and also the purpose of the codebase. Doing machine learning with Python is one of the places, where specialized, on prem hardware resources could be a necessity. But for deploying a webservice (backend for a site for example) cloud deployment seems more natural.