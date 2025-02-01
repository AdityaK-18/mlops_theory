Chapter 1

### **Short Notes on Python 101 for Interview**

#### **Introduction**
- Covers Python basics from installation to data manipulation in Pandas.
- Serves as a refresher for experienced users and a foundation for beginners.

#### **Topics Covered**
- **Installation**: Python setup on Windows, Mac, and Linux.
- **Basic Syntax**: Running Python programs (Hello World!).
- **Data Structures**: List, Tuple, Dictionary, Set, Array, and String.
- **Control Flow**: if-else, loops (for, while), and pass statement.
- **Functions**: Built-in and user-defined functions.
- **OOP (Object-Oriented Programming)**: Class, Object, Methods, `__init__`, `self`.
- **NumPy**: Numerical operations, array handling, reshaping.
- **Pandas**: DataFrames, data manipulation, selection, aggregation, file handling.

#### **Key Concepts**
- **Installation**: Use Python 3.6.10 and maintain a consistent version.
- **Code Editors**: Preferred – Visual Studio Code, others – Sublime Text, Notepad++.
- **Hello World!**: First Python program using `print()`.
- **Data Structures**:
  - **List**: Ordered, mutable collection `[]`.
  - **Tuple**: Ordered, immutable collection `()`.
  - **Dictionary**: Key-value pairs `{}`.
  - **Set**: Unordered, unique elements `{}`.
  - **Array**: Homogeneous data using `array` module.
  - **String**: Text representation in single (`'`) or double (`"`) quotes.

- **Control Statements**:
  - **if-else**: Decision-making based on conditions.
  - **for loop**: Iterates over sequences.
  - **while loop**: Executes until the condition is met.
  - **pass**: Placeholder for future code.

- **Functions**:
  - Built-in: `print()`, `len()`, etc.
  - User-defined: `def function_name():`

- **OOP Concepts**:
  - **Class**: Blueprint for objects.
  - **Object**: Instance of a class.
  - **Methods**: Functions inside classes.
  - **__init__()**: Constructor for initialization.
  - **self**: Refers to instance attributes.

- **NumPy**:
  - Supports multi-dimensional arrays.
  - Faster computations for large datasets.
  - `reshape()` and `flatten()` for array transformations.

- **Pandas**:
  - Used for data manipulation and analysis.
  - DataFrame for tabular data.
  - Methods: `.head()`, `.tail()`, `.describe()`, `.groupby()`.
  - File Handling: `.to_csv()`, `.to_excel()` for saving data.

#### **Points to Remember**
- Maintain the same Python version throughout a project.
- `__init__()` is used for automatic initialization in classes.
- Tuples are immutable, except for mutable elements inside them.

---

### **Interview Questions**

#### **Basic Python Questions**
1. What are the key differences between a list and a tuple?
2. How do you install Python on different operating systems?
3. What is the purpose of the `pass` statement in Python?
4. What are the common data structures in Python?
5. How do you run a Python script from the terminal?
6. Explain the difference between `print()` and `return` in a function.

#### **Control Flow & Functions**
7. How does an `if-else` statement work in Python?
8. What is the syntax of a `for` loop and a `while` loop?
9. What is the significance of the `__init__()` method in Python?
10. How do you define and call a function in Python?

#### **Object-Oriented Programming (OOP)**
11. What is Object-Oriented Programming (OOP)?
12. Explain the difference between a class and an object.
13. What is the role of the `self` keyword in Python classes?
14. How does method overriding work in Python?

#### **NumPy & Pandas**
15. What are the advantages of using NumPy over lists in Python?
16. How do you create a NumPy array and reshape it?
17. What is the difference between `.loc[]` and `.iloc[]` in Pandas?
18. How do you read and write CSV files using Pandas?

#### **Miscellaneous**
19. What are some commonly used Python editors?
20. What are the benefits of using Anaconda for Python development?

These questions will help in assessing Python fundamentals, control flow, OOP concepts, and data handling capabilities. Let me know if you need more details! 🚀

Chapter 2:
### **Short Notes on Git and GitHub for Interview**

## **1. Introduction to Git and GitHub**
- Git is a **Distributed Version Control System (DVCS)** that helps developers manage code versions.  
- **GitHub** is a cloud-based platform for **storing, collaborating, and managing Git repositories**.
- Git allows **multiple developers** to work on the same project while keeping track of changes.

## **2. Key Concepts**
- **Version Control**: Tracks file changes over time.  
- **Commit**: Saves changes with a message for future reference.  
- **Branching**: Creates separate code versions without affecting the main project.  
- **Merging**: Combines changes from different branches.  
- **Push & Pull**: Transfers changes between local and remote repositories.  

---

### **Q1. What is the difference between Git and GitHub?**  
**A:**  
| Feature | Git | GitHub |
|---------|----|--------|
| Type | Command-line tool | Web-based platform |
| Purpose | Version control system | Hosting for Git repositories |
| Collaboration | Works locally | Enables team collaboration |
| Internet Required? | No | Yes |

---

## **3. Installing Git and Creating a GitHub Account**
### **Installation Steps**
- **Linux (Ubuntu/Debian)**
  ```bash
  sudo apt-get update
  sudo apt-get install git
  ```
- **Windows & macOS**: Download from [Git official site](https://git-scm.com/downloads).

- **To check installation**:
  ```bash
  git --version
  ```

### **Q2. How do you create a GitHub account?**  
1. Go to [GitHub Signup](https://github.com/join).  
2. Provide email, username, and password.  
3. Verify email and sign in.  

---

## **4. Common Git Workflow**
The standard workflow includes:
1. **Initialize repository** (`git init`)
2. **Stage files** (`git add filename`)
3. **Commit changes** (`git commit -m "message"`)
4. **Push to GitHub** (`git push origin branch_name`)

### **Q3. What is the command to initialize a new repository?**  
**A:**  
```bash
git init
```
This command **creates a new Git repository** in the current directory.

---

## **5. Common Git Commands**
### **Configuration**
- Set global username:
  ```bash
  git config --global user.name "Your Name"
  ```
- Set global email:
  ```bash
  git config --global user.email "your@email.com"
  ```

### **Q4. What is the command to check the status of files in Git?**  
**A:**  
```bash
git status
```
It shows:
- Tracked and untracked files
- Staged and unstaged changes
- The current branch status

---

### **6. Working with Files in Git**
| **Command** | **Description** |
|------------|---------------|
| `git add [file]` | Stages a file for commit |
| `git commit -m "message"` | Saves the changes |
| `git push origin [branch]` | Uploads local changes to GitHub |
| `git pull origin [branch]` | Fetches updates from GitHub |
| `git clone [repo_url]` | Copies a remote repository |

### **Q5. How do you upload changes to a remote Git repository?**  
**A:**  
```bash
git push origin main
```
It pushes **local commits** to the **main** branch on GitHub.

---

### **7. Branching and Merging**
- **Branching** allows working on new features separately.
- **Merging** integrates branch changes into the main branch.

#### **Creating a Branch**
```bash
git branch feature-branch
git checkout feature-branch
```
#### **Merging Branch**
```bash
git checkout main
git merge feature-branch
```

### **Q6. What is the command to switch to another branch?**  
**A:**  
```bash
git checkout branch_name
```

---

### **8. Rolling Back and Reverting Changes**
- **View commit history**
  ```bash
  git log
  ```
- **Undo last commit**
  ```bash
  git reset --soft HEAD~1
  ```
- **Undo staged files**
  ```bash
  git reset HEAD filename
  ```
- **Restore a file**
  ```bash
  git checkout -- filename
  ```

### **Q7. How do you revert a commit in Git?**  
**A:**  
```bash
git revert commit_id
```
It **creates a new commit** that reverses the changes from the specified commit.

---

## **9. Cloning a Repository**
- **Clone an existing GitHub repository**
  ```bash
  git clone repo_url
  ```
- It **creates a copy** of the repository on the local machine.

### **Q8. How do you clone a repository from GitHub?**  
**A:**  
```bash
git clone https://github.com/user/repo.git
```

---

## **10. GitHub Actions**
- Automates **CI/CD (Continuous Integration & Deployment)**.
- Runs **tests and builds** automatically after code changes.

---

### **Conclusion**
- **Git** is a command-line tool for version control, while **GitHub** is a cloud-based collaboration platform.
- Git allows **tracking changes**, **branching**, and **merging code**.
- Understanding **Git commands** is essential for software development teams.

---

### **Key Points to Remember**
✅ Git **tracks file changes** and allows version control.  
✅ `git init` initializes a new repository.  
✅ `git commit -m "message"` saves changes.  
✅ `git push origin main` uploads changes to GitHub.  
✅ `git pull origin main` fetches updates from the remote repository.  
✅ `git clone URL` downloads a project.  
✅ `git status` shows file tracking status.  

---

### **Interview Questions with Answers**
#### **1. What is Git, and how is it different from GitHub?**  
✅ **Git** is a version control system for tracking code changes.  
✅ **GitHub** is a cloud-based platform that hosts Git repositories for collaboration.  

#### **2. What is the command to upload changes to the remote repository?**  
✅ `git push origin main`  

#### **3. How do you roll back changes in Git?**  
✅ `git revert commit_id` (Creates a new commit to undo changes)  
✅ `git reset --hard commit_id` (Removes changes completely)  

#### **4. How do you initialize a new Git repository?**  
✅ `git init`  

#### **5. What does `git status` do?**  
✅ Shows the current state of the working directory (tracked, untracked, staged files).  

#### **6. How do you create and switch to a new branch in Git?**  
✅ `git branch new-branch` (Creates a new branch)  
✅ `git checkout new-branch` (Switches to new branch)  

#### **7. What is the command to see the commit history?**  
✅ `git log`  

#### **8. How do you merge a branch into the main branch?**  
✅ `git checkout main`  
✅ `git merge feature-branch`  

#### **9. How do you clone a GitHub repository?**  
✅ `git clone repo_url`  

#### **10. What is GitHub Actions?**  
✅ A CI/CD tool for automating software workflows on GitHub.  

---

This structured format will **help in interviews** with clear **concepts, commands, and Q&A**. Let me know if you need more! 🚀

Chapter 3:

Got it! I'll now explain **ML Model Deployment Challenges** in a structured way, just like before, with **short notes** followed by **interview questions and answers**.

---

# **Short Notes on Challenges in ML Model Deployment**

## **1. Introduction**
- **87% of ML models never reach production** due to deployment challenges.  
- ML model deployment depends on:
  - **Prediction frequency** (real-time or batch)
  - **Latency requirements**
  - **Number of users**
  - **Infrastructure & accessibility**  
- **MLOps** (Machine Learning Operations) helps streamline the ML lifecycle by automating deployment and monitoring.

---

## **2. ML Life Cycle** *(Refer to Figure 3.1)*
The **ML lifecycle** involves **multiple stages**:

1. **Business Impact** – Define how ML will impact revenue, cost, or efficiency.
2. **Data Collection** – Gather structured/unstructured data from multiple sources.
3. **Data Preparation** – Clean, transform, and format data.
4. **Feature Engineering** – Extract useful features to improve model performance.
5. **Build & Train Model** – Select, train, and optimize machine learning algorithms.
6. **Test & Evaluate** – Validate model accuracy, precision, and recall.
7. **Model Deployment** – Deploy the trained model for real-world use.
8. **Monitoring & Optimization** – Track performance and retrain models when needed.

💡 *Example:* If a model performs below expectations, it may require **feature engineering improvements** or **hyperparameter tuning** before deployment.

---

## **3. Challenges in ML Model Deployment**
### **A. Data Challenges**
- **Data is scattered** across multiple databases and formats.
- **Data inconsistency** (missing values, duplicate records, noise).
- **3Vs of Data**: 
  - **Volume** (large datasets),
  - **Velocity** (data is constantly changing),
  - **Variety** (structured, unstructured data).  
- **Data Storage** issues in handling and managing large datasets.

### **B. Model Challenges**
- **Selecting the right model** for scalability and efficiency.
- **Computational power** required for training deep learning models.
- **Overfitting vs. Underfitting** affecting generalization.
- **Model drift** – Performance degrades over time as data changes.

### **C. Deployment Challenges**
- **Portability issues** – Model runs differently across environments.
- **Scalability concerns** – Model must handle **increased user traffic**.
- **Integration issues** – Connecting ML models with **existing applications and databases**.
- **Security threats** – Adversarial attacks, data poisoning.

---

## **4. Types of ML Model Deployment**
### **1. Batch Predictions**
- Model processes data in bulk and stores predictions in a database.
- Used in **reporting systems, analytics dashboards**.
- **Example:** Predicting customer churn monthly.

💡 *Pros:*  
✅ Simple & cost-effective.  
💡 *Cons:*  
❌ Not suitable for real-time applications.  

### **2. Web Service (REST API)**
- Model is deployed as an **API** that processes **single records in real-time**.
- Used in **chatbots, fraud detection, recommendation engines**.

💡 *Pros:*  
✅ Easy to integrate into mobile/web apps.  
💡 *Cons:*  
❌ Latency issues with high request loads.  

### **3. Edge/Mobile Deployment**
- Model runs **directly on devices** (smartphones, IoT sensors, cameras).
- Used in **voice assistants, smart home devices**.

💡 *Pros:*  
✅ Works without an internet connection.  
💡 *Cons:*  
❌ Limited hardware resources.  

### **4. Real-Time Prediction**
- Model processes **live streaming data** for **immediate decisions**.
- Used in **stock market analysis, autonomous vehicles, fraud detection**.

💡 *Pros:*  
✅ Immediate insights with low latency.  
💡 *Cons:*  
❌ Expensive to maintain infrastructure.  

---

## **5. MLOps – Machine Learning Operations** *(Refer to Figure 3.3)*
- **MLOps = Machine Learning + DevOps + Data Engineering**.
- Bridges the gap between **ML model training and deployment**.
- Uses **CI/CD pipelines** to **automate ML lifecycle**.
- **Monitors model drift** and **automatically retrains models**.
- Ensures **scalability, security, and reproducibility**.

### **MLOps Components**
| **Component** | **Purpose** |
|--------------|------------|
| **CI/CD Pipelines** | Automates training & deployment |
| **Model Monitoring** | Detects accuracy drop & retrains |
| **Infrastructure Management** | Ensures scalability |
| **Version Control** | Tracks model updates |

---

## **6. Benefits of MLOps**
### **1. Efficient ML Lifecycle Management**
- Automates **model training, testing, and deployment**.
- **Example:** If model accuracy drops, **MLOps triggers retraining automatically**.

### **2. Reproducibility**
- Ensures **consistent results** across different environments.
- Uses **Docker & Kubernetes** to **deploy models reliably**.

### **3. Automation**
- Reduces manual intervention in **testing, scaling, monitoring**.
- Ensures **fast deployment with minimal errors**.

### **4. Model Tracking & Feedback Loop**
- Monitors performance and **alerts teams if accuracy drops**.
- **Example:** If model accuracy falls **below 70%**, retraining is triggered.

---

## **Interview Questions & Answers**

### **Q1. What are the major challenges in ML model deployment?**
✅ **Data Challenges** – Scattered, inconsistent, and large datasets.  
✅ **Model Challenges** – Computational power, overfitting, model drift.  
✅ **Deployment Challenges** – Portability, scalability, integration, security risks.  

---

### **Q2. How does MLOps differ from DevOps?**
| **Feature** | **DevOps** | **MLOps** |
|------------|-----------|-----------|
| Code Type | Static | Dynamic (Models retrain) |
| Deployment | One-time | Continuous updates |
| Monitoring | Focuses on system performance | Focuses on model drift & accuracy |

---

### **Q3. What are different ways to deploy ML models?**
✅ **Batch Predictions** – Processes multiple records at once.  
✅ **Web Service (REST API)** – Provides real-time predictions.  
✅ **Edge/Mobile Devices** – Runs ML models locally.  
✅ **Real-Time Prediction** – Processes streaming data instantly.  

---

### **Q4. How does MLOps solve ML deployment issues?**
✅ **Automates ML lifecycle** with CI/CD pipelines.  
✅ **Monitors performance** to detect model drift.  
✅ **Ensures reproducibility** across different environments.  
✅ **Enhances security** against adversarial attacks.  

---

### **Q5. What is model drift, and how do you handle it?**
✅ **Model drift** occurs when an ML model’s accuracy degrades due to **changing data patterns**.  
✅ **Handling drift:**  
- Monitor performance using logging tools.  
- Retrain the model with fresh data.  
- Use adaptive learning to update model weights dynamically.  

---

### **Q6. What are the benefits of using REST API for ML deployment?**
✅ **Scalability** – Handles multiple requests simultaneously.  
✅ **Flexibility** – Integrates easily with mobile/web apps.  
✅ **Real-time predictions** – Delivers instant results.  

---

### **Q7. What is the role of Continuous Integration (CI) & Continuous Deployment (CD) in MLOps?**
✅ **CI:** Automates testing and validation of ML models.  
✅ **CD:** Ensures models are deployed automatically after passing quality checks.  

---

## **Conclusion**
- **Deploying ML models is challenging** due to **data, scalability, and security issues**.
- **MLOps automates the ML lifecycle** and ensures **efficient deployment**.
- **Monitoring and retraining are essential** to maintain model performance.
- **Different deployment methods** (batch, REST API, edge devices) depend on business needs.

---

This structured **short notes + Q&A format** is perfect for interviews. Let me know if you need any modifications! 🚀

Chapter 4:

# Packaging ML Models

## **Introduction**
Machine Learning (ML) models need to be packaged efficiently to ensure easy deployment, maintainability, and reusability. This chapter covers the essential steps to modularize Python code and build ML packages that can be installed and used on other machines or servers.

---
## **Structure**
This chapter covers:
- 🔹 **Virtual Environment**
- 🔹 **Requirements File**
- 🔹 **Serializing & Deserializing ML Models**
- 🔹 **Testing Python Code using Pytest**
- 🔹 **Python Packaging & Dependency Management**
- 🔹 **Developing, Building, and Deploying ML Packages**
- 🔹 **Setting Up Environment Variables and Paths**

---
## **Objectives**
✅ Learn to create and activate virtual environments.
✅ Install dependencies and package ML models.
✅ Save trained ML models using pickling.
✅ Test and debug Python packages using `pytest`.
✅ Understand Python packaging and dependency management.

---
## **1️⃣ Virtual Environments**
A **virtual environment** isolates dependencies for different projects. This is helpful when different projects require different versions of the same package.

📌 **Install Virtual Environment:**  
```sh
pip install virtualenv
```

📌 **Create a Virtual Environment:**  
```sh
virtualenv venv_project
```

📌 **Activate Virtual Environment:**  
```sh
source venv_project/bin/activate  # Mac/Linux
venv_project\Scripts\activate  # Windows
```

📌 **Deactivate Virtual Environment:**  
```sh
deactivate
```

📌 **List Installed Packages:**  
```sh
pip list  # OR
pip freeze
```

---
## **2️⃣ Requirements File**
The `requirements.txt` file holds the list of dependencies required for a project.

📌 **Generate a requirements file:**  
```sh
pip freeze > requirements.txt
```

📌 **Install dependencies from requirements file:**  
```sh
pip install -r requirements.txt
```

---
## **3️⃣ Serializing & Deserializing ML Models**
Serialization (pickling) allows saving ML models for reuse. **Joblib** is a popular library for this purpose.

📌 **Install Joblib:**  
```sh
pip install joblib
```

📌 **Save ML Model:**  
```python
import joblib
joblib.dump(model, 'model.pkl')
```

📌 **Load Saved Model:**  
```python
loaded_model = joblib.load('model.pkl')
```

---
## **4️⃣ Testing Python Code with Pytest**
Testing ensures that your package functions correctly before deployment.

📌 **Install Pytest:**  
```sh
pip install pytest
```

📌 **Run Pytest:**  
```sh
pytest -v
```

📌 **Example Test Case:**  
```python
import pytest

def test_sum():
    assert sum([1, 2, 3]) == 6
```

📌 **Output Indicators:**  
- ✅ `.` – Test Passed
- ❌ `F` – Test Failed
- ⚠️ `E` – Error Occurred

---
## **5️⃣ Python Packaging & Dependency Management**
Modularizing Python code helps improve maintainability and reusability.

📌 **Components of a Python Package:**
- `module.py`: A Python file containing functions/classes.
- `package/`: A directory with multiple modules.
- `__init__.py`: Marks a directory as a package.

📌 **Example Package Structure:**
```
📦 prediction_model/            # Root directory (ML Model Packaging)
│── 📜 MANIFEST.in             # File manifest for package distribution
│── 📖 README.md               # Documentation about the package
│── 📜 requirements.txt        # List of dependencies for installation
│── ⚙️ setup.py                 # Setup script for package installation
│
├── 📂 prediction_model/        # Main package directory
│   ├── 📜 __init__.py          # Initializes this directory as a Python package
│   ├── ⚙️ config.py             # Configuration settings, constants, and paths
│   ├── 🔗 pipeline.py          # Defines the ML pipeline steps
│   ├── 🔮 predict.py           # Loads the model and performs predictions
│   │
│   ├── 📂 processing/           # Data processing utilities
│   │   ├── 🛠 data_management.py # Handles data loading, saving, and transformations
│   │   ├── 🎭 preprocessors.py   # Custom preprocessing functions (encoding, scaling, imputation)
│   │
│   ├── 📂 trained_models/       # Folder for storing trained ML models
│   │   ├── 🏆 model.pkl         # Serialized trained ML model (Pickle format)
│   │
│   ├── 🎯 train_pipeline.py     # Script to train the ML model and save it
│
└── 📂 tests/                    # Unit testing directory
    ├── ⚙️ pytest.ini             # Pytest configuration file
    ├── 🧪 test_predict.py       # Unit test cases for the prediction module

```

---
## **6️⃣ Developing, Building, & Deploying ML Packages**
### **Business Problem: Loan Approval Prediction**
A company wants to automate loan eligibility based on customer details. The dataset includes factors like income, loan amount, credit history, etc.

📌 **Steps to Build ML Package:**
1. **Prepare dataset** (cleaning, processing, feature engineering).
2. **Build and train model** (store trained model as `.pkl` file).
3. **Package modules** (include `config.py`, `pipeline.py`, etc.).
4. **Write test cases** (`pytest` for validation).
5. **Create `setup.py` for installation.**

📌 **Install Package Locally:**  
```sh
pip install -e .
```

📌 **Install from GitHub:**  
```sh
pip install git+https://github.com/username/repository.git
```

---
## **7️⃣ Setting Up Environment Variables & Paths**
Environment variables help in specifying paths dynamically.

📌 **Add to `.bashrc` or `.bash_profile`:**  
```sh
echo "export PYTHONPATH=/home/user/project:$PYTHONPATH" >> ~/.bashrc
source ~/.bashrc
```

---
## **Conclusion**
✔ Virtual environments help isolate dependencies.  
✔ `requirements.txt` ensures consistency across machines.  
✔ **Pickling & Joblib** allow saving ML models.  
✔ `pytest` ensures robust testing before deployment.  
✔ Modular programming improves **reusability** and **debugging**.  
✔ Python packaging simplifies sharing ML models.  

---
## **Key Terms**
🔹 **PYTHONPATH** – Specifies directories to be searched for Python modules.  
🔹 **Joblib** – Used for model persistence.  
🔹 **Pickling** – Saving Python objects as files.  
🔹 **Manifest.in** – Lists files to include/exclude in packages.  
🔹 **Setup.py** – Used to build Python packages.  

Chapter 5: 
# MLflow - Platform to Manage the ML Life Cycle

## Introduction
The Machine Learning (ML) life cycle involves multiple challenges, such as:
- Trying different models with various parameters and hyperparameters.
- Keeping track of the best-performing model and its parameters.
- Saving the serialized model for reusability.

MLflow is a platform designed to streamline ML development by **tracking experiments, managing models, and deploying them efficiently**.

---

## Structure
This document covers:
- Introduction to MLflow
- MLflow Tracking
- MLflow Projects
- MLflow Models
- MLflow Model Registry

---

## Objectives
By the end of this guide, you should be able to:
- Train, reuse, and deploy ML models using MLflow.
- Track model evaluation metrics and hyperparameters.
- Save trained models using serialization techniques.
- Compare models visually using MLflow UI.
- Deploy models and consume them via APIs.

---

# Introduction to MLflow
**MLflow** is an **open-source platform** for managing the **end-to-end ML life cycle**.

### Key Features:
✔️ Tracks model evaluation metrics like RMSE, AUC, accuracy.
✔️ Saves trained models along with hyperparameters.
✔️ Deploys models to production or cloud environments.
✔️ Maintains version control over models in staging and production.
✔️ Supports multiple ML libraries and languages (Python, R, Java, etc.).
✔️ Provides a **UI** to compare models side by side.
✔️ Offers integration with tools like REST APIs and CLI.

---

## Setting up MLflow Environment
### Install Miniconda (if not already installed)
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

### Create and Activate Virtual Environment
```bash
conda create -n venv python=3.7
conda activate venv
```

### Install MLflow
```bash
pip install mlflow
```

To check MLflow installation:
```bash
mlflow --help
```

Start MLflow UI:
```bash
mlflow ui
```
The UI should open at `http://localhost:5000`.

---

# MLflow Components
MLflow consists of four primary components:
1. **MLflow Tracking** - Logs metrics, parameters, and artifacts.
2. **MLflow Projects** - Packages ML code with dependencies.
3. **MLflow Models** - Stores and serves ML models.
4. **MLflow Model Registry** - Manages model versions and transitions.

Each of these components is independent but can work together.

---

## MLflow Tracking
MLflow Tracking captures the following information:
✅ **Run Metadata** - Start & end times, source files.
✅ **Parameters** - Hyperparameters like `n_estimators`, `max_depth`.
✅ **Metrics** - Model performance (e.g., Accuracy, F1-score).
✅ **Artifacts** - Saved files such as trained models, plots, logs.

### Logging Parameters and Metrics
```python
import mlflow

# Set tracking URI (Local or Remote Server)
mlflow.set_tracking_uri('http://localhost:5000')

# Start a new run
with mlflow.start_run(run_name="Loan_Prediction_Model"):
    mlflow.log_param("n_estimators", 100)
    mlflow.log_metric("accuracy", 0.85)
    mlflow.set_tag("model_version", "0.1.0")
    mlflow.end_run()
```

### Logging Artifacts (e.g., CSVs, Model Files)
```python
import pandas as pd

# Save dataset as CSV
data = pd.DataFrame({'Cust_id': [101,102,103], 'Sales': [5000,7000,8000]})
data.to_csv("customer_sales.csv", index=False)

# Log CSV as artifact
mlflow.log_artifact("customer_sales.csv")
```

To retrieve the **artifact URI**:
```python
mlflow.get_artifact_uri()
```

---

# Building an ML Model with MLflow
## Dataset: Loan Prediction
```python
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split, GridSearchCV
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.tree import DecisionTreeClassifier
from sklearn import metrics
import mlflow

# Load dataset
data = pd.read_csv("loan_dataset.csv")
num_col = data.select_dtypes(include=['int64','float64']).columns.tolist()
cat_col = data.select_dtypes(include=['object']).columns.tolist()
cat_col.remove('Loan_Status')
cat_col.remove('Loan_ID')

# Fill missing values
for col in cat_col:
    data[col].fillna(data[col].mode()[0], inplace=True)
for col in num_col:
    data[col].fillna(data[col].median(), inplace=True)

# Feature engineering
data['TotalIncome'] = data['ApplicantIncome'] + data['CoapplicantIncome']
data.drop(['ApplicantIncome','CoapplicantIncome'], axis=1, inplace=True)

# Label encoding
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
for col in cat_col:
    data[col] = le.fit_transform(data[col])
data['Loan_Status'] = le.fit_transform(data['Loan_Status'])

# Train-test split
X = data.drop(['Loan_Status', 'Loan_ID'], axis=1)
y = data['Loan_Status']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)

# Train model
rf = RandomForestClassifier(n_estimators=100, max_depth=5, random_state=42)
rf.fit(X_train, y_train)

# Log model with MLflow
with mlflow.start_run():
    mlflow.log_params({"n_estimators": 100, "max_depth": 5})
    mlflow.log_metric("accuracy", metrics.accuracy_score(y_test, rf.predict(X_test)))
    mlflow.sklearn.log_model(rf, "random_forest_model")
    mlflow.end_run()
```

---

# MLflow Models and Deployment
## Serving Model as REST API
```bash
mlflow models serve -m "runs:/<RUN_ID>/random_forest_model" --port 1234
```

## Calling Model via API
```bash
curl -X POST -H "Content-Type: application/json" --data '{"data": [[1,1,0,1,0,4.85,360,1,2,8.67]]}' http://127.0.0.1:1234/invocations
```

---

# MLflow Model Registry
MLflow **Model Registry** allows versioning and transitioning models from **Staging** to **Production**.

```python
mlflow.register_model("runs:/<RUN_ID>/random_forest_model", "Loan_Prediction_Model")
```

Change model status:
```python
mlflow.transition_model_version_stage("Loan_Prediction_Model", version=1, stage="Production")
```

---

# Conclusion
✅ **MLflow is a powerful tool** for tracking, versioning, and deploying ML models.
✅ It supports **hyperparameter tuning**, **artifact storage**, and **API deployment**.
✅ **MLflow UI provides visual insights** into different model runs.
✅ **Model Registry helps in versioning** and maintaining production-ready models.

---






