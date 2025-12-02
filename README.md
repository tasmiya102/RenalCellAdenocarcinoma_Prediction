Early detection of Renal Cell Carcinoma (RCC) significantly increases a patient’s chances of receiving timely and effective treatment. Traditional diagnostic procedures are often labor-intensive, time-consuming, and reliant on specialized expertise. To address this, we developed a machine learning–powered prediction system that identifies the likelihood of RCC at an early stage using routine blood test results.

The system is built around a Random Forest Classifier that analyzes patient biomarkers to generate accurate predictions. It is fully integrated into a responsive web application, enabling users and healthcare professionals to easily input data and receive instant results.

The project uses a dual-backend design:

Flask serves as the backend for handling machine learning inference.

MySQL manages user authentication and data storage, with SQLAlchemy acting as the ORM bridge between the application and database.

This combination ensures secure data handling, seamless communication between components, and fast, reliable predictions — ultimately reducing diagnostic delays, lowering costs, improving precision, and easing the workload on medical personnel.

🚀 Features
🧪 ML model (RandomForestClassifier) trained on clinical blood test parameters
🌐 Interactive web interface for easy data input
🔐 User authentication system (signup, login, stored history)
🗄 Dual-backend architecture
    -Flask handles ML inference
    -MySQL stores user data
🔗 SQLAlchemy ORM connects Flask with MySQL
⚡ Instant RCC prediction
📊 Model retraining capability


🛠️ Tech Stack
Languages & Libraries

Python

scikit-learn (RandomForestClassifier)

SQLAlchemy

Pandas / NumPy

Backend

Flask (ML inference backend)

MySQL (user data backend)

Frontend

HTML

CSS

JavaScript

Other Tools

SQLAlchemy ORM

REST API

Virtual environment (venv)

# steps to run:
**#Clone the Repository**
git clone https://github.com/tasmiya102/RenalCellAdenocarcinoma_Prediction.git
cd RenalCellAdenocarcinoma_Prediction
**Create and Activate Virtual Environment**
python -m venv venv

**Windows**
venv\Scripts\activate

**Install Required Packages**
pip install -r requirements.txt

**Set Up MySQL Database**
Install and start MySQL
Create a new database:
CREATE DATABASE rcc_prediction;
Update the database URI in your Flask config:
mysql+pymysql://username:password@localhost/rcc_prediction

**Initialize Database Tables**
flask db upgrade

**Run the Application**
python app.py

# DEMO
<h1>HOME PAGE</h1>
![Home Page](https://raw.githubusercontent.com/tasmiya102/RenalCellAdenocarcinoma_Prediction/main/Screenshot%20(3).png)

<h1>CHECKUP PAGE</h1>

![CHECK UP](https://github.com/tasmiya102/RenalCellAdenocarcinoma_Prediction/blob/main/Screenshot%20(5).png)

<h1>RESULT </h1>

![RESULT](https://github.com/tasmiya102/RenalCellAdenocarcinoma_Prediction/blob/main/Screenshot%20(6).png)

<h1>APPOINTMENT BOOKING FORM</h1>

![APPOINTMENT](https://github.com/afra-af/RenalCellAdenocarcinoma_Detection/assets/81957946/603f6103-a655-4126-a9fb-bb7048774af7)

<h1>CONTACT US PAGE</h1>
![CONTACT](https://github.com/tasmiya102/RenalCellAdenocarcinoma_Prediction/blob/main/Screenshot%20(4).png)
