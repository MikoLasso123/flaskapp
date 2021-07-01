# RAD Full Stack Tech Assessment

### Introduction

This Technical assessment is part of the interviewing process for a Full Stack Development position in the RAD Unit at Ipsos Public Affairs.

Feel free to complete those tasks in any way you choose.

We are expecting your solution to be in python 3.6 or higher.

Please give high attention to development community standards when writing your code. This may include:

> -   Limiting your code line to a reasonable length.
> -   Including Doc Strings and type hinting where applicable.
> -   Your code should be self-explanatory.
> -   Adding comments where you think we need clarification.
> -   Breaking down your code into folders, and files properly.
> -   Grouping issues into features and tackling them through Git branches.
> -   Submitting pull requests with appropriate comments.
> -   Submitting different commits to show the logical flow of your code.

We are excited to go through your code and learn about your coding skills.

* * *

## Task

You are asked to build the data pipeline backend for a quick dashboard that can give the user an overall view on COVID-19 epidemiological indicators across the US.

### Product Requirements

1. As a user I want to know the current total number of active cases and deaths on the country and state level.
2. As a user I want to see an epidemiological indicator trend chart where I can compare national trends to states. I should be able to choose between active cases and deaths.
3. As a user I want to know the bi-weekly percentage of change (increase/drop) in the epidemiological indicator of interest on the national or state levels.
4. As a user I want to get the most recent reported number of deceased or active cases on the national level or for each state.
5. As a user I want to identify the top 5 states with highest value in term of totals for the epidemiological indicator of interest.

### Coding Requirements

You are required to deliver a working, tested, and ready for deployment code.

For testing, please include your testing code in the repo. For deployment, we recommend wrapping your code in docker containers that includes all the environment requirements for your code to run. Yet, feel free to use any different approaches you think is better for your code to work.

Also, the code will be deployed and tested on AWS. If you believe your API will better work on a lambda function please give us the list of requirements for the lambda env to have it deployed in a lambda instead.

### Steps (Optional)

**1: Data Extraction, Transformation, and Load:**

In this step you will need to pull the data from an outside source and get it ready for exhibition.

> -   Pull the epidemiological data provided by [Novel COVID-19 API](https://disease.sh/docs/#/) for the US.
> -   Process and transform the data to the format you see appropriate for storage.
> -   Use the provided MySQL database instance in the config file to store the data.
> -   You will need to structure your relational database to get it ready for storage.

**2: BackEnd API:**

In this step you need to build a BackEnd API to allow for data consumption. The API should be ready to handle different scenarios to satisfy the user stories, meaning it receives certain parameters to give us the expected data.
We are expecting the API to comply with the REST framework requirements. All the API responses should be in JSON format and should be ready for display with no further manipulation on the frontend side.

> -   Connect your BackEnd to the given relational database.
> -   Build your aggregation code to prepare data for delivery.
> -   Note that, your dashboard should be up to date to the latest data provided by the Novel COVID-19 API at all times.

_N.B. these steps are optional. Feel free to use the approach you see appropriate for your code to work_

### Documentation

Depending on your code and your delivery, we require that you provide documentation for it. For instance, if you went with building an API, please include a README file that explains how to use it including

> -   Endpoint.
> -   Data Formats.
> -   Available Parameters.
> -   Other stuff you think are important.

Also, for the MySQL relational database, please provide a data catalog for your relational design including

> -   Table names.
> -   Table fields names and descriptions.
> -   Entity relationship diagram.
> -   Other stuff you think are important to include.

Finally, if you decided to use either docker containers or lambdas for deployment, please include a document to explain

> -   Steps for deployment.
> -   Expected Configuration requirements.
