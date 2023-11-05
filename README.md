# 03_fedex

In the notebook `03_fedex.ipynb` there is analysis delivery data of Fedex. The additional visualization and overall summary can be found [here](https://bayan2019.github.io/03_fedex_html/)

Managers at Fedex have to evaluate a lot of factors before taking a decision of delivery.
The objective of this project is to optimize the process of planning delivery.

Objective(s): Maximize the security of deliveries.

Constraints: Minimize disappointments of lost. Restricted computational power.

Success Criteria:

- Business Success Criteria: Reduce the number of lost packages between 30% to 55%

- Economic Success Criteria: Fedex will see a decrease in lost by at least 30%

Proposed Plan:
Classification of deliveries will allow to understand the characteristics of each group.

There was provided a big dataset or 3 604 175 package delivery records.

Actions performed:
- Deleting missing values and duplicates. Since the data is big, there was no need for any imputation techniques.
- Instead of year, month, day of month and day of week, there was engineered the date column.
- Deleting outliers and Balancing Dataset. We had much more undelivered packages (2 804 071) than delivered (718092).
- Performed typecasting -- converted some variables from 'float' to 'integers'
- Performed Exploratory Data Analysis which can be briefly considered here https://bayan2019.github.io/03_fedex_html/index.html
- Carried out normality check for numerical variables (they all do not have normal distribution)
- Scaled numerical features.
- Conducted One-hot encoding.
- Build 4 models -- K Nearest Neighbors, Naive Bayes, Logistic Regression, and Decision Tree.
- After evaluation of 4 models Decision Tree was selected as the best model.