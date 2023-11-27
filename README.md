# 2023 UNF AI4Good Hackathon Project

## Overview
This project, developed during the AI4Good Hackathon at the University of North Florida, aimed to tackle the challenge of enhancing participant retention in FirstTee, particularly among youth aged 12 and older.

## About FirstTee
FirstTee is an organization focused on youth development through golf, especially in lower-income communities. The organization faces a challenge with declining participation rates as children grow older, especially those aged 12 and above. Our project addresses this issue.

## Problem Statement
Understanding and mitigating the decline in participation rates among older children in First Tee programs.

## Our Solution
### Predictive Modelling
- We employed machine learning algorithms, including an SGD classifier and a random forest model, to predict participant retention.
- The initial models showed perfect prediction metrics due to data leakage, which we identified and corrected after the hackathon.

### Interactive Web Application
- We built an interactive web application to supplement our predictive models.
- The application displays detailed information on FirstTee chapters, such as average participants, session prices, and retention rates, helping users identify trends in chapters with low retention rates.

## Technical Challenges and Learnings
- We faced a significant challenge with data leakage in our initial models. The same variable used to determine retainment in 2022 was inadvertently used in training the model, leading to perfect metrics.
- Post-hackathon, we revised our approach to eliminate this data leakage and ensure more accurate model predictions.
- Initially, we planned to integrate various AWS applications into our solution. However, due to various technical errors, we were unable to utilize these tools as intended.
- Despite these challenges, we are grateful for the support and mentorship provided by AWS throughout the hackathon. Their guidance was invaluable in navigating these obstacles and in the overall development of our project.

## Repository Structure
### Data
- Description
    - Includes CSV files of all datasets.
- Contents
    - *chapter-data.csv*: information about FirstTee chapters
    - *listing-sessions-2018-2020.csv*: information about sessions within each FirstTee chapter
    - *participant-data.csv*: information about FirstTee participants
    - *program-locations.csv*: information about session and program locations
    - *session-registration.csv*: information about individual sessions
    - *data-preprocessed-EDA.csv*: created after preprocessing raw data; used to conduct EDA
    - *data-preprocessed-modeling.csv*: created after preprocessing raw data; used to train model

### Notebooks
- Description
    - Includes Jupyter Notebooks used in project.
- Contents
    - *data-preprocessing.ipynb*: data preprocessing
    - *exploratory-data-analysis.ipynb*: EDA on preprocessed data
    - *modeling.ipynb*: model training

### Results
- Description
    - Includes results from models and exploratory data analysis
- Contents
    - *age-year-distributions.png*: plot representing age and year distributions
    - *correlation-matrix.png*: correlation matrix
    - *ethnicity-distribution.png*: plot representing ethnicity distribution
    - *gender-distribution.png*: plot representing gender distribution
    - *sessions-price-duration-distributions.png*: plot representing session rate, price rate, and session duration rate distributions
    - *model-metrics.csv*: table representing basic metrics for models
    - *forest-predictions.csv*: random forest model predictions
    - *forest-cross-validation.txt*: random forest model cross validation scores
    - *feature-importances.csv*: random forest model feature importances
    - *sgd-predictions.csv*: sgd classifier predictions
    - *sgd-cross-validation.txt*: sgd classifier cross validation scores
    - *roc-curve.png*: plot representing ROC curve for both models
    - *trained-randomforest.joblib*: joblib file representing trained random forest model
    - *trained-sgdclassifier.joblib*: joblib file representing trained sgd classifier

### Web App
- Description
    - Includes files to run web application
- Contents
    - HTML, CSS, and JavaScript files that follow a template that create our web application

### .gitignore
- Purpose: to exclude unnecessary files, environments

### requirements.txt
- Purpose: to indicate package versions used

## Data Confidentiality and Dummy Data
- For confidentiality reasons, the project uses dummy data in place of actual participant data from FirstTee.

## Installation and Setup

To get this project up and running on your local machine, follow these steps:

### Prerequisites
- Ensure you have Python 3.9.6 installed on your machine. You can download it from [Python's official site](https://www.python.org/downloads/)
- An understanding of basic Python programming and data science concepts is beneficial.

### Clone the Repository
1. Clone the project repository to your local machine using Git:

`git clone https://github.com/m-ryan-nugent/ai4good-hackathon-2023.git`

### Set up a virtual environment (optional, but recommended)
2. Navigate to the project directory:

`cd ai4good-hackathon-2023`

3. Create a virtual environment to manage your project dependencies separately:

`python -m venv venv`

4. Activate the virtual environment:
- On Windows: `venv\Scripts\activate`
- On macOS and Linux: `source venv/bin/activate`

### Install Required Dependencies
5. Install the required Python packages using `pip`:

### Running the Application
6. To run the web application:
- Open `starter.html` file with web browser.

## Support
For any further assistance, feel free to contact me at my [email](mryannugent@gmail.com).

## Acknowledgements
- We extend our heartfelt thanks to the AI4Good Hackathon organizers (Drs. Umapathy and Richard), mentors, and FirstTee.
- Special appreciation goes to my teammates, Walid and Michael, for their data science expertise, innovative solutions, and for creating a friendly and enjoyable environment during my first hackathon.
- We also express our gratitude to Spencer from FirstTee for continuing to help the participants through the various technical issues.

## License
- This project does not require a specific license due to the use of dummy data for confidentiality.

## Contact
- Mark Nugent [n01174983@unf.edu](n01174983@unf.edu)
- Michael Kimollo [n01542707@unf.edu](n01542707@unf.edu)
- Walid Kambagha [n01531675@unf.edu](n01531675@unf.edu)
