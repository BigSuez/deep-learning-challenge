# Deep Learning Challenge

## Tools Used:
- Jupyter Notebook
- SKLearn
- Pandas
- TensorFlow
- Keras Tuner

## Report:
### Overview:
  - The goal this project is to assist a Non-Profit Foudnation that helps fund various ventures. Using Machine Learning and Neural Networks, create a model that will help them assess if a given application will be successful or not.
### Results:
  - Data Preproccesing:
    - The Target Variable for this Dataset is the success of previously funded applicants. Labeled as IS_SUCCESFUL
    - The Features Variables for this Dataset include:
      - Application Type
      - Affiliation
      - Classification
      - Use Case
      - Organization Type
      - Income Amount
      - Ask Amount
    - Other Removed Variables for this Dataset include:
      - Applicant Name
      - Applicant EIN
  - Evaluation:
    - The most effective model found consisted of 3 Hidden Layers, with 9, 5, and 9 Neurons respectively.
    - I was unable to acheive the target 75% Predictive Accuracy, ending up with a maximum of |||||||
    - Some of the steps attempted to increase model accuracy:
      - Removing low-impact columns (Special Considerations, Status, Organization, Use Case). Every attempt at removing columns yielded lower accuracy
      - Decreasing Number of Bins. This led to lower accuracy.
      - Increasing Number of Bins. This led to a slightly higher accuracy, but not enough to be functionally useful.
      - Adding Hidden Layers. This fairly consistantly lowered accuracy beyond 2 layers.
      - Removing Hidden Layers. Moving to 1 Hidden Layer slightly lowered accuracy.
      - Keras Tuner. Finally, I decided to use Keras Tuner to find the optimal HyperParamaters. This yielding slightly better results, but still under the target 75%.
  - Summary:
    - While I ended up with a ||||| Predictive Accuracy, I hit a road-block getting it any higher with the current data. The model would still prove useful, as it can lower the amount of hands-on time required for particularly good or bad applications, but it will still require a good amount of manual oversight. One obvious but expensive way to improve this model would be having more data, either as more applicants or more data per applicant. More realistically, different models beyond Keras Sequential may yield better results. Alternatively, having more time or computing power to run a more in-depth Keras Tuner may give more insight into optimal hyper-parameters. Overall, while my model had moderate success, I do not beleive it to be the ideal model for this use-case.


  -Bryson
