# Vehicle Classification: Model Comparison

Trains and compares three classifiers on a large vehicles listings dataset (about 1.4 GB CSV), then publishes the scores on a small results website.

Built for the Introduction to Data Mining course, M.Sc. Computer Science, Syrian Virtual University.

## Results

| Metric | Logistic Regression | Decision Tree | Naive Bayes |
|---|---|---|---|
| Accuracy | 0.2543 | **0.6377** | 0.0609 |
| Precision | 0.1192 | **0.6378** | 0.1801 |
| Recall | 0.2543 | **0.6377** | 0.0609 |
| F1-score | 0.1519 | **0.6376** | 0.0189 |

The Decision Tree is the clear winner. It handles the mix of categorical and numeric vehicle attributes without scaling or encoding assumptions, while Logistic Regression and Naive Bayes struggle with the many classes and correlated features.

## Code

The full analysis is in the [Colab notebook](https://colab.research.google.com/drive/1S9EiWhpOG03Yjv0ZTEjq-70NLGLUQHVQ?usp=sharing). The dataset is not included because of its size.

## Results site

`IDM/public_html/idm/IDM.html` shows the scores. Built with HTML, SCSS and Bootstrap; `npx gulp` serves it locally.
