
# Portfolio Part 3 - Analysis of Mobile Price Data (2024 S1)


### Introduction:
Welcome to the third part of our portfolio project focusing on the analysis of mobile price data. In this task, we delve into the intricate details of mobile phone specifications and prices, aiming to build predictive models that categorize mobile phones into different price ranges. The dataset provides a rich source of information, including hardware specifications such as battery power, camera quality, memory, and network support, which are crucial factors influencing mobile phone prices in the market.

Our objective is to explore this dataset, clean the data, select relevant features, and train machine learning models to accurately predict the price range of mobile phones. By leveraging various classification algorithms such as logistic regression and K-nearest neighbors (KNN), we aim to gain insights into the relationship between mobile phone specifications and prices. Additionally, we employ techniques such as hyperparameter tuning using GridSearchCV to optimize model performance and enhance prediction accuracy.

Throughout this project, we strive to provide a comprehensive analysis of the mobile price data, elucidating the factors driving mobile phone prices and the effectiveness of different machine learning approaches in predicting price ranges. Our ultimate goal is to equip stakeholders in the mobile industry with actionable insights that can inform pricing strategies, product development decisions, and market positioning strategies.



## Data Overview:

### Dataset Description:
The Mobile Price Data dataset contains comprehensive information about mobile phone hardware specifications and prices. It includes various features such as battery power, camera quality, memory, and network support, along with the corresponding price ranges categorized as low, medium, high, and very high.

### Features:
The dataset comprises the following features:

- **Battery Power:** Total energy a battery can store in one time measured in mAh.
- **Bluetooth:** Binary attribute indicating the presence of Bluetooth support.
- **Clock Speed:** Speed at which the microprocessor executes instructions.
- **Dual SIM:** Binary attribute indicating the presence of dual SIM support.
- **Front Camera (FC):** Mega pixels of the front camera.
- **4G:** Binary attribute indicating the presence of 4G network support.
- **Internal Memory:** Internal memory capacity in gigabytes.
- **Mobile Depth (M dep):** Depth of the mobile phone in centimeters.
- **Mobile Weight:** Weight of the mobile phone.
- **Number of Cores (N cores):** Number of processor cores.
- **Primary Camera (PC):** Mega pixels of the primary camera.
- **Pixel Height (Px height):** Pixel resolution height.
- **Pixel Width (Px width):** Pixel resolution width.
- **RAM:** Random access memory capacity in megabytes.
- **Screen Height (Sc h):** Screen height of the mobile phone in centimeters.
- **Screen Width (Sc w):** Screen width of the mobile phone in centimeters.
- **Talk Time:** Longest time that a single battery charge will last during use.
- **3G:** Binary attribute indicating the presence of 3G network support.
- **Touch Screen:** Binary attribute indicating the presence of a touch screen.
- **Wi-Fi:** Binary attribute indicating the presence of Wi-Fi support.
- **Price Range:** The target variable indicating the price range of the mobile phone (0: low cost, 1: medium cost, 2: high cost, 3: very high cost).

### Data Cleaning:
Before proceeding with the analysis, the dataset undergoes a data cleaning process, which includes:
- Handling missing values.
- Removing abnormal instances and outliers.
- Ensuring data consistency and integrity for robust analysis and modeling.



### Getting Started:
To get started with this project, follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine using the following command:
   ```
   git clone <repository_url>
   ```
2. **Install Dependencies**: Ensure you have Python installed on your machine. Install the required dependencies using pip:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
3. **Download Dataset**: Download the "Mobile Price Data" dataset (CSV format) from the provided source or website.
4. **Set Up Environment**: Place the downloaded dataset in the project directory.

### Dependencies:
The following libraries are used for data analysis and machine learning tasks:
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn


### Data Analysis Steps:
1. **Data Exploration and Cleaning**: Explore the dataset, address missing values, and eliminate abnormal instances or outliers to ensure data cleanliness.
2. **Feature Selection**: Analyze the correlation between the price range and other features to select variables conducive to prediction.
3. **Dataset Splitting**: Split the dataset into training and testing sets in an 80:20 ratio for subsequent model training and evaluation.

### Logistic Regression Model:
- **Description**: Logistic regression is a linear model used for binary classification tasks. In this project, it's employed to predict price ranges based on selected features.
- **Implementation**: The logistic regression model is trained using the Scikit-learn library, with accuracy evaluated on both training and test sets.
- **Model Evaluation**: High accuracy on both training and test sets indicates effective learning and generalization.

### KNN Model:
- **Description**: K-nearest neighbors (KNN) is a non-parametric classification algorithm used for pattern recognition. It predicts the price range by finding the most common class among the K nearest neighbors.
- **Implementation**: The KNN model is trained using Scikit-learn, with K set to an ad-hoc value initially.
- **Model Evaluation**: Robust performance with minimal overfitting is observed, indicating effective classification of mobile phones into price categories.

### Hyperparameter Tuning and GridSearchCV:
- **Description**: Hyperparameter tuning aims to find the optimal values for parameters that are not directly learned during model training. GridSearchCV exhaustively searches over specified parameter values to find the best combination.
- **Implementation**: GridSearchCV is used to tune the hyperparameter K in the KNN model. It evaluates the model's performance using cross-validation and selects the best K value based on the mean accuracy score.
- **Outcome**: The best K value is identified, enhancing the model's accuracy and effectiveness in price range prediction.



## Model Performance Evaluation:

Both logistic regression and K-nearest neighbors (KNN) models show strong performance in predicting the price range of mobile phones based on selected features.

- **Logistic Regression:** Achieves high training accuracy of **95.56%** and a slightly higher test accuracy of **97.17%**. The model effectively learns the relationship between features like RAM, battery power, and price range.

- **K-Nearest Neighbors (KNN):** With an ad-hoc value of K=5, the model demonstrates robust performance with a training accuracy of **94.78%** and a test accuracy of **92.54%**. Hyperparameter tuning using GridSearchCV identifies the optimal K value as 13, achieving a mean test score of approximately **93.11%**.

--- 


