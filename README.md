# final project

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Final project for INST414: the topic is the preditors/determinants of adolescent mental health. Focusing on finding predictors for mental health based on public mental health datasets.

### Core Dependencies:

```
Python 3.8+
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
pytest
```

### Installation
Clone the Repository
```
git clone [(https://github.com/EricTanUMD/414-project)]
```
Activate Virtual Environment
```
source path/to/venv/bin/activate  # Linux/macOS
path\to\venv\Scripts\activate     # Windows
```
Install Dependencies
```
pip install -r requirements.txt
```

### Dataset

This project utilizes the "Depression and Mental Health Data Analysis" dataset from Kaggle, which contains survey responses focused on mental health factors and depression indicators among adolescents and young adults.

### Dataset Details
- **Source**: https://www.kaggle.com/datasets/bhavikjikadara/mental-health-dataset/data
- **Format**: CSV files containing survey response data
- **Size**: Approximately 300k raws

### Key Variables
- Age: Represents the age of the participants.
- Gender: Indicates the gender of the participants.
- Occupation: Represents the participant's occupations.
- Days_Indoors :Indicates the number of days the participant has not been out of the house
- Growing_Stress: Indicates the participant's stress is increasing day by day (Yes/No).
- Quarantine_Frustration: Frustrations in the first two weeks of quarantine (Yes/Maybe/No).
- Changes_Habits: Represents major changes in eating habits and sleeping (Yes/Maybe/No).
- Mental_Health_History : A precedent of mental disorders in the previous generation (Yes/No).
- Weight_Change :Highlights changes in body weight during quarantine (Yes/Maybe/No)
- Mood_Swings: Represents extreme mood changes (Low/Medium/High).
- Coping_Struggles: The inability to cope with daily problems or stress (Yes/Maybe/No).
- Work_Interest :Represents whether the participant is losing interest in working (Yes/No).
- Social_Weakness :Conveys feeling mentally weak when interacting with others (Yes/No).

The raw data is stored in `data/raw/`, with processed versions available in `data/processed/` 

## Planned Modeling Approach
The following modeling techniques are planned for future implementation:
- Logistic regression to identify key determinants of depression and anxiety
- Random forest classifiers to detect patterns of mental health risk factors
- Feature importance analysis to rank determinants by their impact

### Model Evaluation Strategy
Models will be evaluated using multiple metrics to ensure comprehensive assessment:
- Accuracy: Overall correctness of predictions
- Sensitivity/Recall: Ability to correctly identify adolescents with mental health concerns
- Specificity: Accuracy in identifying those without mental health concerns
- Precision: Proportion of positive identifications that are actually correct
  
### License
Distributed under the MIT License. See LICENSE.txt for more information.

### Acknowledgments
Kaggle for providing the dataset

### Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         project and configuration for tools like black
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`


--------

