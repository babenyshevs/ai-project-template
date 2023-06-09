# <*Project-name*>

# AI Project Requirements Mind Map

## Project Overview
- Business value:
  - *Helpful questions to ask/answer:*
    - *What are business KPIs?*
    - *How to let business-customer shine as a result of the project?*
    - *Bottle-necks:*
      - *"We want to be data-driven" often means: "We already made a decision and now want you to confirm it with data"*
      - *AI is not needed or business ment by it something alse, e.g.:*
        - *fix business process*
        - *solve data engineering task*
        - *solve data analytics task*
    - *Good candidates for applying AI:*
      - *Repetitive tasks*
      - *Tasks involving processing of large ammount of data*
      - *Tasks which are currently solved only partially*
      - *Task which business fails to deliver properly for long time*
      - *Tasks on which budget reduction is expected*
- Business objectives:
  - Business metric *- very important!*
  - AI team transforms business metric into a technical evaluation (used for development and evaluation)
- Expected Outcomes (options):
  - PoC
  - MVP
  - Full scale solution

## Stakeholders
- Project Sponsors (budget)
- Users 
- Developers
  - *Data engineer*
  - *Data analyst*
  - *Data scientist / ML Engineer / MLOps engineer*
- Other Relevant Parties

## Functional Requirements
- Data Collection and Preprocessing
  - Data sources
  - Data access
  - Data requiremnts:
    - Types
    - Formats
    - Ammount (expecially if subsample is provided)
    - Stability (devset should not differ from live data)
    - Quality (missings, migtrating schema, etc)

- Quality metrics
  - Desired level of quality (prediction accuracy)
  - Continuous improvement (if aplicable)

- Inference and Prediction
  - Batch vs. Realtime
  - Output destination

- Integration and Deployment
  - Integrate with existing systems and applications
  - CI/CD

- Performance
  - Large volumes of data
  - Processing time limits
  - Minimal latency (for real-time applications)

- Usability
  - Interface (if aplicable)
  - Documentation
    - Git README
    - Confluence

## Non-Functional Requirements
- Model Training and Validation
  - Justify modelling methodology - what kind of task is to be solved
  - Justify model architecture - how it will be solved (target definition, etc.)
  - Experiments tracking

- Security
  - Data confidentiality and integrity
  - Access control

- Scalability
  - Handle increasing data and users
  - Horizontal and vertical scaling

- Monitoring and Maintenance
  - Include monitoring and logging mechanisms
  - Track performance and identify issues
  - Support regular updates and maintenance
## Constraints and Assumptions
- Programming language
  - Python
  - Spark
  - SQL
- Infrastructure (premise, cloud, mix)
- Access to data
  - Classification
  - User roles

## Dependencies
- External libraries, frameworks, or data sources

## Acceptance Criteria
- Measurable criteria for project completion

## Deliverables
- 1. Documentation
- 2. Artifacts
      - Trained models
      - Deployment scripts
    - DB & Tables
    - Reports
    - WebApp

## Timeline and Milestones
- Project timeline with major milestones

## Risks and Mitigation
- Identified risks and strategies for mitigation


## Code & structure
### Directory structure
------------

The directory structure of your new project looks like this: 

```
├── README.md               <- The top-level README for developers using this project.
├── data
│   ├── external            <- Data from third party sources.
│   ├── interim             <- Intermediate data that has been transformed.
│   ├── processed           <- The final, canonical data sets for modeling.
│   └── raw                 <- The original, immutable data dump.
│
├── logs                    <- Log API requests (e.g. input, response, stdout, stderr information)
│
├── docs                    <- A default Sphinx project; see sphinx-doc.org for details
│
├── models                  <- Trained and serialized models, model artifacts, or model summaries
│
├── notebooks               <- Jupyter notebooks. Naming convention is a number (for ordering),
│                              the creator's initials, and a short `-` delimited description, e.g.
│                              `1.0-sa-initial-data-exploration`.
│
├── references              <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports                 <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures             <- Generated graphics and figures to be used in reporting
│
├── requirements.txt        <- The requirements file for reproducing the analysis environment, e.g.
│                              generated with `pip freeze > requirements.txt`
│
├── src                     <- Source code for use in this project.
│   ├── __init__.py     <- Makes src a Python module
│   │
│   ├── config.py       <- Configuration file for some global variables
│   │
│   ├── data            <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features        <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models          <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict.py
│   │   └── train.py
│   │
│   └── visualization   <- Scripts to create exploratory and results oriented visualizations
│           └── visualize.py
│
├── tests                   <- Test scripts for unit testing (e.g. using pytest), 
│                              performance and load testing of the API
│
├── api.py                  <- Flask API script
│
└── .gitignore
```

### Backup
#### Q&A
- Q: What this activity seek to achieve (i.e. MLOps seminar, etc)?
  - A: More AI use cases in production
    - Q: how many there are now?
  - A: Faster delivery?
    - Q: how long it takes now?
    - Q: how fast we want it to be?
  - A. Better quality if AI use cases
    - Q: what is the quality now?
    - Q: how to we measure it?
    - Q: does it need to be higher?
- Q: What are success criteria (how to measure success)?
  - A:
- Q: Till when?
  - A:

#### Next steps:
- [ ] Implement this template in Production use cases (Team Digimon, S2P Hub)
- [ ] Present template in Data Science communitys
- [ ] ...
- [ ] Step N


#### Installing development requirements
------------

    pip install -r requirements.txt

#### Running the tests
------------

    pytest tests

#### Build documentation using Sphinx
------------

    cd docs/
    make html
