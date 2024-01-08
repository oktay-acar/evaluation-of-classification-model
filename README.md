# Evaluation of Classification Model

### Project Tasks

### Task 1: 
A classification model has been created that predicts whether the customer is churn or not. The actual values ​​of 10 test data observations and the probability values ​​predicted by the model are given.
- Create a **confusion matrix** by taking the threshold value to **0.5**.
- Calculate **Accuracy**, **Recall**, **Precision**, **F1 Scores**.

| &nbsp; | Actual Value | Model Probability Estimation *(probability of belonging to class 1)* |
| :----: | :----------: | :----------------------------------------------------------------: |
|   1    |      1       |                                0.7                                 |
|   2    |      1       |                                0.8                                 |
|   3    |      1       |                                0.65                                |
|   4    |      1       |                                0.9                                 |
|   5    |      1       |                                0.45                                |
|   6    |      1       |                                0.5                                 |
|   7    |      0       |                                0.55                                |
|   8    |      0       |                                0.35                                |
|   9    |      0       |                                0.4                                 |
|   10   |      0       |                                0.25                                |


<table> 
<tbody>
 <tr>
    <th rowspan='6'>Actual Value</th>
 </tr>
 <tr>
  <th colspan='5'>Model Prediction</th>
 </tr>
 <tr>
  <td colspan='2'>&nbsp;</td>
  <td>Non-Churn (0)</td>
  <td>Churn (1)</td>
  <td>&nbsp;</td>
 </tr>
 <tr>
  <td colspan='2'>Non-Churn (0)</td>
  <td>?</td>
  <td>?</td>
  <td>?</td>
 </tr>
 <tr>
  <td colspan='2'>Churn (1)</td>
  <td>?</td>
  <td>?</td>
  <td>?</td>
 </tr>
 <tr>
  <td colspan='2'>&nbsp;</td>
  <td>?</td>
  <td>?</td>
  <td>&nbsp;</td>
 </tr>
</tbody>
</table>

### Task 2: 
A classification model has been created in order to detect fraudulent transactions during transactions made through the bank. The success of the model with **90.5% accuracy rate** was found to be sufficient and the model was taken live. However, after going live, the output of the model was not as expected, and the business unit reported that the model was unsuccessful. The **confusion matrix** of the **prediction results** of the model is given below. According to this;
- Calculate **Accuracy**, **Recall**, **Precision**, **F1 Scores**.
- Comment on what the **'Data Science'** team may have overlooked.

<table> 
<tbody>
 <tr>
    <th rowspan='6'>Actual Value</th>
 </tr>
 <tr>
  <th colspan='5'>Model Prediction</th>
 </tr>
 <tr>
  <td colspan='2'>&nbsp;</td>
  <td>Non-Fraud (0)</td>
  <td>Fraud (1)</td>
  <td>&nbsp;</td>
 </tr>
 <tr>
  <td colspan='2'>Non-Fraud (0)</td>
  <td>900</td>
  <td>90</td>
  <td>990</td>
 </tr>
 <tr>
  <td colspan='2'>Fraud (1)</td>
  <td>5</td>
  <td>5</td>
  <td>10</td>
 </tr>
 <tr>
  <td colspan='2'>&nbsp;</td>
  <td>905</td>
  <td>95</td>
  <td>&nbsp;</td>
 </tr>
</tbody>
</table>

- **True Negative (TN):** 900
- **False Positive (FP):** 90
- **True Positive (TP):** 5
- **False Negative (FN):** 5

---

## Requirements
~~~python
matplotlib==3.7.1
numpy==1.24.3
pandas==1.5.1
seaborn==0.12.1
sklearn==1.3.1
~~~

---

## Author
[Oktay Acar](https://github.com/oktay-acar)