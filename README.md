# <*Project-name*>

# AI Project Requirements Mind Map

## Project Overview
- Purpose
- Business objectives - metrics
- Expected Outcomes

## Stakeholders
- Project Sponsors (budget)
- Users 
- Developers
- Other Relevant Parties

## Functional Requirements
- Data Collection and Preprocessing
  - Data sources
  - Data access

- Model Training and Evaluation
  - Justify modelling methodology - what kind of task is to be solved
  - Justofy model architecture - how it will be solved (target definition, etc.)
  - Experiments tracking

- Inference and Prediction
  - Batch vs. Realtime
  - Output destination

- Integration and Deployment
  - Integrate with existing systems and applications
  - CI/CD

- Monitoring and Maintenance
  - Include monitoring and logging mechanisms
  - Track performance and identify issues
  - Support regular updates and maintenance

## Non-Functional Requirements
- Performance
  - Large volumes of data
  - Processing time limits
  - Minimal latency (for real-time applications)

- Quality metrics
  - Desired level of quality (prediction accuracy)
  - Continuous improvement (if aplicable)

- Security
  - Data confidentiality and integrity
  - Access control

- Scalability
  - Handle increasing data and users
  - Horizontal and vertical scaling

- Usability
  - Interface (if aplicable)
  - Documentation

## Constraints and Assumptions
- Programming language
- Infrastructure (premise, cloud, mix)
- Access to data

## Dependencies
- External libraries, frameworks, or data sources

## Acceptance Criteria
- Measurable criteria for project completion

## Deliverables
- Trained models
- Deployment scripts
- Documentation and artifacts

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
├── models                  <- Trained and serialized models, model predictions, or model summaries
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

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    pytest tests

### Build documentation using Sphinx
------------

    cd docs/
    make html
