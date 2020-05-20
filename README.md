# Data Analysis in SQL <br/>by **Michel Semaan**

Live training sessions are designed to mimic the flow of how a real data scientist would address a problem or a task. As such, a session needs to have some “narrative” where learners are achieving stated learning objectives in the form of a real-life data science task or project. For example, a data visualization live session could be around analyzing a dataset and creating a report with a specific business objective in mind _(ex: analyzing and visualizing churn)_, a data cleaning live session could be about preparing a dataset for analysis etc ... 

As part of the 'Live training Spec' process, you will need to complete the following tasks:

Edit this README by filling in the information for steps 1 - 4.

## Step 1: Foundations 

This part of the 'Live training Spec' process is designed to help guide you through session design by having you think through several key questions. Please make sure to delete the examples provided here for you.

### A. What problem(s) will students learn how to solve? (minimum of 5 problems)

- Organizing query results in CTEs.
- Using joins to compare historical data.
- Using window functions to fetch values from other rows.
- Converting dates to a human-readable format.
- Extract meaningful insights from data in SQL.

### B. What technologies, packages, or functions will students use? Please be exhaustive.

- `JOIN`
- `DATE_TRUNC`
- `ROUND`
- CTEs (`WITH ___ AS ___`)
- `LAG`

### C. What terms or jargon will you define?

- Common table expressions (CTEs) are temporary tables that store a query's results so that they can be used in a subsequent query while avoiding complex subqueries.
- Window functions look at certain rows related to the current row and apply operations on them like fetching, sliding, and paging.

### D. What mistakes or misconceptions do you expect? 

- CTEs are temporary tables; they're destroyed as soon as the query finishes running.
- Window functions always operate based on the window defined in them.

### E. What datasets will you use? 

Live training sessions are designed to walk students through something closer to a real-life data science workflow. Accordingly, the dataset needs to accommodate that user experience. 
As a rule of thumb, your dataset should always answer yes to the following question: 
> Is the dataset/problem I’m working on, something an industry data scientist/analyst could work on? 

Check our [datasets to avoid](https://instructor-support.datacamp.com/en/articles/2360699-datasets-to-avoid) list. 

## Step 2: Who is this session for?

Terms like "beginner" and "expert" mean different things to different people, so we use personas to help instructors clarify a live training's audience. When designing a specific live training, instructors should explain how it will or won't help these people, and what extra skills or prerequisite knowledge they are assuming their students have above and beyond what's included in the persona.

- [X] Please select the roles and industries that align with your live training. 
- [X] Include an explanation describing your reasoning and any other relevant information. 

### What roles would this live training be suitable for?

*Check all that apply.*

- [ ] Data Consumer
- [ ] Leader 
- [X] Data Analyst
- [X] Citizen Data Scientist
- [ ] Data Scientist
- [ ] Data Engineer
- [X] Database Administrator
- [ ] Statistician
- [ ] Machine Learning Scientist
- [ ] Programmer
- [ ] Other (please describe)

The course would be suited for anyone who connects to SQL databases to analyze data therein.

### What industries would this apply to?

*List one or more industries that the content would be appropriate for.*

- E-commerce
- Streaming
- Retail

### What level of expertise should learners have before beginning the live training?

*List three or more examples of skills that you expect learners to have before beginning the live training*

> - Can use SELECT statements to fetch desired data from a table.
> - Can JOIN tables together.
> - Can calculate grouped summary statistics using SELECT queries with GROUP BY clauses.
> - Can use basic SQL functions to modify results.

## Step 3: Prerequisites

List any prerequisite courses you think your live training could use from. This could be the live session’s companion course or a course you think students should take before the session. Prerequisites act as a guiding principle for your session and will set the topic framework, but you do not have to limit yourself in the live session to the syntax used in the prerequisite courses.

- Introduction to SQL
- Joining Data in SQL

## Step 4: Session Outline

A live training session usually begins with an introductory presentation, followed by the live training itself, and an ending presentation. Your live session is expected to be around 2h30m-3h long (including Q&A) with a hard-limit at 3h30m. You can check out our live training content guidelines [here](_LINK_). 

### Introduction Slides 
- Introduction to the webinar and instructor (led by DataCamp TA)
- Introduction to the topics
  - Stress the ubiquity of SQL databases
  - Discuss how dashboarding and reporting tools plug into SQL
  - Mention how writing data analysis queries in SQL plays into that
  - Set expectations about Q&A
### Live Training
#### Preparing the data
- Explore the table's schema 
- Define basic terms like DAU (daily active users) and MAU (monthly active users)
- Use `GROUP BY` to calculate them
- **Q&A** 
#### User retention and churn
- Getting which month each user was active in
- Joining a previous month to a subsequent month to see whether the user churned
- Calculate monthly retention and churn rates 
#### User growth
- Using a CTE to store MAU
- Using `LAG` to fetch the previous month's MAU
- Calculating MAU growth
- **Q&A**
### Ending slides
- Recap of what we learned
- Why data analysis in SQL
- Call to action and course recommendations

## Authoring your session

To get yourself started with setting up your live session, follow the steps below:

1. Download and install the "Open in Colabs" extension from [here](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo?hl=en). This will let you take any jupyter notebook you see in a GitHub repository and open it as a **temporary** Colabs link.
2. Upload your dataset(s) to the `data` folder.
3. Upload your images, gifs, or any other assets you want to use in the notebook in the `assets` folder.
4. Check out the notebooks templates in the `notebooks` folder, and keep the template you want for your session while deleting all remaining ones.
5. Preview your desired notebook, press on "Open in Colabs" extension - and start developing your content in colabs _(which will act as the solution code to the session)_.  :warning: **Important** :warning: Your progress will **not** be saved on Google Colabs since it's a temporary link. To save your progress, make sure to press on `File`, `Save a copy in GitHub` and follow remaining prompts. You can also download the notebook locally and develop the content there as long you test out that the syntax works on Colabs as well.
6. Once your notebooks is ready to go, give it the name `session_name_solution.ipynb` create an empty version of the Notebook to be filled out by you and learners during the session, end the file name with `session_name_learners.ipynb`. 
7. Create Colabs links for both sessions and save them in notebooks :tada: 
