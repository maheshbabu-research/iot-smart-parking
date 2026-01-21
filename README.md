# IoT Based Smart Parking Management

**Project Objective:**

This project aims to harness the power of **IoT enabled Smart Parking system** and uses prediction 
algorithms to predict and optimize Parking using the real-time dataset collected from IoT-enabled 
parking facilities.     

**Project Description:**

Smart Parking Management System provides real-time monitoring and management of parking spaces. The application uses data from various IoT sensors to track the occupancy of parking spots, optimize space utilization, and improve the overall parking experience.

We primarily focus on prediction of Parking Slot Availability and 
EV Charging Spot availability based on Machine Learning Models adopted.

This application can be further enhanced to include

**Key functionalities:**

•	Real-time monitoring of parking spots.

•	Notifications about available spots (via mobile apps or dashboards).

•	Dynamic pricing based on occupancy and demand.

•	Data-driven decision-making for parking facility management.

•	Vehicle entry/exit tracking and payment monitoring.

**Users of the system:**

•	Parking Facility Operators: For managing parking spaces, optimizing resource allocation, and monitoring occupancy.

•	Drivers/Users: For receiving notifications about available spots, making reservations, and tracking payment status.

•	City Planners/Urban Developers: To gain insights into parking utilization trends, occupancy patterns, and related infrastructure requirements.

•	Electric Vehicle (EV) Users: To find available EV charging stations and spots.

The IoT application/system fits into the Smart City industry. It provides a real-time solution for managing urban parking infrastructure, optimizing parking space usage, reducing congestion, and improving the efficiency of city transportation networks.

In the **context of Smart Cities**, the application helps improve urban mobility by:

•	Reducing traffic caused by drivers searching for parking.

•	Providing real-time data that can inform urban planning and parking policy decisions.

•	Supporting electric vehicle adoption by offering data on available charging stations.

Additionally, this system could also be valuable in the Transportation and Logistics sector, where efficient space allocation, traffic management, and cost optimization play a critical role.



**Challenges:**

1. **Data Imbalance:**  
   Challenge: Imbalance in data, especially for the Occupancy Status variable, can lead to biased predictions.  
   Solution: Use data balancing techniques like oversampling, undersampling, or algorithms like XGBoost to handle imbalance.

2. **Missing Data:**  
   Challenge: Incomplete or missing data points, such as Sensor Readings or Payment Status, hinder model accuracy.  
   Solution: Apply imputation techniques or models capable of handling missing data effectively.

3. **Feature Correlation:**  
   Challenge: Correlated features, like Parking Duration and Occupancy Status, may cause multicollinearity in the model.  
   Solution: Use feature engineering or dimensionality reduction methods like PCA to minimize redundancy.

4. **Noisy Data:**  
   Challenge: Sensor data and environmental noise can interfere with model predictions.  
   Solution: Clean the data using preprocessing techniques like smoothing or filtering.

5. **Real-Time Data Processing:**  
   Challenge: Real-time prediction of parking or charging availability requires fast processing with minimal latency.  
   Solution: Use edge computing for real-time inference to reduce latency and ensure quick predictions.

6. **External Factors:**  
   Challenge: External factors like weather or traffic conditions are difficult to incorporate and may be inconsistent.  
   Solution: Integrate external data sources (e.g., APIs for weather and traffic) into the models in real-time.


**Methods Used:**

  - IoT - Real-time dataset having readings from sensors
    
  - Exploratory Data Analysis (EDA) process to analyze the real-time IoT dataset
    
  - Machine Learning for Parking Slot Availability and EV Charging Availability Prediction
    
  - Time Series Methods for Predicting Parking Slot Availability and EV Charging Availability Prediction
    
  - Data Visualization - Charts and Report in Tableau
    
  - Data Manipulation - Augmenting using synthetic data

**Technologies:**
  - Machine Learning / Time Series - Linear Regression, LSTM, XGBoost
  - Tableau for Visualization and Report
  - Python Libraries: TensorFlow, PyTorch, NumPy, Matplotlib, Scikit-learn

  **Frameworks:** PyTorch, TensorFlow

  **IDE:** Google Colab, VS Code


**Dataset:**
    
The source of the dataset is an IoT-enabled parking management system deployed across parking 
facilities. It collects real-time data from various sensors, including proximity, pressure, and ultrasonic 
sensors, along with data on parking occupancy, weather conditions, vehicle types, and traffic 
patterns. This system is likely connected to a cloud platform or local servers that store and process 
the data, making it accessible for analysis.

**Dataset Statistics**
  
  **Selected Dataset:** Smart Parking Management Dataset - https://www.kaggle.com/datasets/datasetengineer/smart-parking-management-dataset?resource=download
  
The dataset contains 1000 records (observations). Each record corresponds to an individual event or 
change in the parking system, such as a vehicle entering or exiting a parking spot, occupancy 
changes, or status updates for specific parking spots. The dataset spans from January 2021 to June 
2024, covering a wide range of time periods. 


The dataset contains the following features/variables: 
1. Timestamp: Date and time of each event. 
2. Parking Spot ID: Unique identifier for each parking spot. 
3. Occupancy Status: Whether the parking spot is occupied or vacant. 
4. Vehicle Type: Type of vehicle parked (car, motorcycle, electric vehicle, etc.). 
5. License Plate Information: Anonymized vehicle license plate data for tracking. 
6. Parking Duration: Duration of time the vehicle is parked. 
7. Entry and Exit Times: The times when vehicles enter and exit the parking lot. 
8. Payment Status: Whether the parking fee has been paid. 
9. Weather Conditions: Data on temperature, precipitation, and humidity. 
10. Nearby Traffic Conditions: Traffic flow and congestion levels around the parking facility. 
11. Occupancy Rate: Percentage of total spots occupied. 
12. Proximity to Entrance/Exit: Distance of parking spots to the lot’s entrances or exits. 
13. Electric Vehicle Charging Availability: Status of charging stations. 
14. Parking Spot Size: Dimensions of the parking spots (standard, compact, oversized). 
15. Sensor Readings: Data from proximity, pressure, and ultrasonic sensors. 
16. User Type: Identification of users (registered, visitor, staff). 
17. Parking Lot Section: Designation of areas within the parking facility (e.g., Zone A, Level 1). 
18. Dynamic Pricing Information: Changes in parking rates based on time or demand. 
19. Reserved Status: Indicates if a spot is reserved. 
20. Environmental Noise Level: Noise levels near parking areas.


**Installation and Execution**

This project is primarily run using either Jupyter Notebook or google colab.
To set up this project

1. **Clone the Repository:**
   Open a terminal and run the following command to clone the repository to your local machine:
   ```bash
   git clone https://github.com/maheshbabu-usd/aai-530-group11-iot-smart-parking
   ```

2. **Navigate to the Project Directory:**
   Change into the project directory:
   ```bash
   cd aai-530-group11-iot-smart-parking
   ```

3. **Setup google colab enviornment**
   Open https://colab.research.google.com using your respective gmail account
   Upload the notebooks into google colab
   Ensure you are using appropriate GPU and High RAM for faster execution
   Setup the Input and Output directories for images and videos in google drive
   
5. **Install Dependencies:**
   Install the required Python packages using `pip`:
   ```bash
   pip install -r requirements.txt
   ```

6. **Run the project notebooks**
   Run in google colab

**References:**

[1] Dataset Source 
https://www.kaggle.com/datasets/datasetengineer/smart-parking-management
dataset?resource=download 

[2] Lookmuang, R., Nambut, K., & Usanavasin, S. (2018). Smart parking using IoT technology. 
Proceedings of the 2018 5th International Conference on Business and Industrial Research (ICBIR), 16. https://doi.org/10.1109/ICBIR.2018.8391155 

[3] Basavaraju, S. R. (2015, December). Automatic smart parking system using Internet of Things 
(IoT). International Journal of Scientific and Research Publications. 
https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=1c92d407c021a829e5d96bf4b1a4b3c575e43f97#page=638



