# Client_Project_Sales
Project Title: Sales Effectiveness Prediction

👤 Client: FicZon Inc.

🎯 Goal: Predict whether a sales lead is high or low potential using machine learning to improve lead prioritization and sales outcomes.

🧪 Exploratory Data Analysis (EDA)

📌 Key Feature Observations:
Product ID:

Products with ID 18, 15, 19, 27, 9, and 5 are the most sold.

Others contribute minimally.

Source:

Most common lead sources: Call, Live Chat, Direct, and Website.

Less than 250 leads from all other sources combined.

Sales Agent:

Top performers: Agent 4, Agent 11, and Agent 5.

Agents 3, 9, and 7 had low sales (< 850).

Location:

Bangalore and Other Locations dominate.

Chennai, Hyderabad, Delhi, and Mumbai trail behind.

Delivery Mode:

Mode 5 is most commonly used.

Modes 2 & 4 are the least used.

Status:

Majority of leads are junk or non-responsive.

High potential leads are a smaller segment.

🧮 Univariate Insights (Percentages Calculated)
21% of customers preferred "Call" source with "Delivery Mode 5".

Only 3% of customers handled by Sales Agent 11 were "Potential".

20% of total customers were "Junk Leads".

44% of customers are from Bangalore.

36% of all sales were for Product ID 18.

Only 0.8% came through Website + Open Status + Agent 10.

🛠️ Preprocessing / Feature Engineering
Missing Value Handling:

Imputed mode for most columns.

Left out features with excessive uniqueness (like email, mobile).

Label Consolidation:

Merged similar or sparse labels in Source, Location, and Status.

Feature Reduction:

Dropped unique/constant columns: Created, Mobile, and EMAIL.

Categorical Encoding:

All string labels encoded to integers using LabelEncoder.

🔍 Correlation Analysis
No highly correlated features detected.

All features are categorical — so limited traditional correlation insight.

🤖 Model Building
You tested KNN, BaggingClassifier (KNN base), and Random Forest.

Applied RandomizedSearchCV to tune the RandomForestClassifier:

Tuned n_estimators, max_depth, min_samples_split, and more.

Best model selected based on F1 Score.

Final evaluation:

Model evaluated on test data using accuracy score.

Likely reported test accuracy and possibly F1 or confusion matrix.

✅ Final Outcome
Completed full EDA → Preprocessing → Modeling → Evaluation workflow.

Successfully predicted lead potential using machine learning.

Built a deployable pipeline that can help FicZon prioritize better leads.

