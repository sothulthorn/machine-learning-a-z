# Model Selection

## K-Fold Cross-Validation

K-Fold Cross-Validation is a model evaluation technique used to assess how well a machine learning model generalizes to unseen data. The dataset is split into **K equal folds**. The model is trained **K times**, each time using **K−1 folds for training** and **1 fold for validation**. The final performance is computed as the **average of all K validation scores**.

This approach provides a more reliable performance estimate than a single train-test split and is widely used in **model selection and hyperparameter tuning**. Common choices are **K = 5 or K = 10**. For classification tasks with imbalanced data, **Stratified K-Fold** is recommended.

## Bias–Variance Tradeoff

The bias–variance tradeoff describes the balance between two sources of error in machine learning models.  
- **Bias** - a systematic error that occurs in the machine learning model itself due to incorrect assumptions in the ML process. Technically, we can define bias as the error between average model prediction and the ground truth.
- **Variance** - how much the model can adjust depending on the given dataset. Variance refers to the changes in the model when using different portions of the training dataset.

### How Bias-Variance Tradeoff works
- **High Bias Low Variance** : The model is *too simple* and does not capture the underlying trend of the data
- **High Bias High Variance**: The model is *too simple* to capture the data's trends and *too sensitive*, capturing noise as well
- **Low Bias Low Variance**: Great model. It accurately captures the underlying trends of the data and generalizes well to unseen data
- **Low Bias High Variance**: The model is *too sensitive* and is capturing noise as if it were a real trend. (overfitting)

## Grid Search

**Grid Search** is a hyperparameter tuning technique used to find the best combination of model parameters. It works by defining a grid of possible hyperparameter values and exhaustively training and evaluating the model for every combination using a validation method such as cross-validation.

Grid Search helps identify optimal hyperparameters but can be computationally expensive for large parameter spaces.
