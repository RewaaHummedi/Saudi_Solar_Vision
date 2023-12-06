# Saudi Solar Vision: Shining Light on tomorrow - T5 bootcamp capstone project

# Introduction: 
This project inteded to to meet the Saudi vision of 2030 and in order to achieve that and increase the efficiency of the solar panels, this project helps in classifying and detecting the status of solar panels in order to get early maintenance or monitoring using Deep learning model with images dataset. also, to predict the generated energy from the solar panel by building machine learning model and a combined dataset consist of power generation data and weather data. furthurmore, a recommendation system that provides the user with 5 other location that is similar with the solar energy based on the location given by the user earlier. Finally, building a customized chatbot that answer any questions related to Saudi project in the field of renewable energy and other solar project. 

# Data Description:

* Image Classification & Detection:
dataset consists of 940 images, 297 images were classified as Clean, 139 images were Electrical Damage,  157 images were Physical Damage, 244 images were Weather Damage, and 103 images were Snow Covered. 

* Energy Prediction:
We used a tabular dataset consist of two files for 34 days that gathered in india and record the sensor data every 15 minutes, the first dataset is the generation power and consist of 7 columns which are DATE_TIME, PLANT_ID, SOURCE_KEY ,DC_POWER, AC_POWER, DAILY_YIELD, TOTAL_YIELD, and 68778 rows. Also, the weather data related to the weather and sun data, consists of 6 columns,DATE_TIME,PLANT_ID,SOURCE_KEY, AMBIENT_TEMP,​ MODULE_TEMP, IRRADIATION, and 3182 rows. In the preprocessing step, we have combined the two dataset to get each module with its weather data, and dropped unnecessary columns 

* Location Recommender:
Specific Photovoltaic Power Output (PVOUT specific):This is a measure of the efficiency of a photovoltaic (PV) system. It represents the amount of electrical energy (in kilowatt-hours, kWh) generated by a system per unit of peak power capacity (kilowatt-peak, kWp).​Direct Normal Irradiation (DNI):DNI refers to the amount of solar radiation received per unit area (in kilowatt-hours per square meter, kWh/m²) by a surface that is always oriented perpendicular to the sun's rays. It measures the direct component of solar irradiance.​Global Horizontal Irradiation (GHI): GHI is the total amount of solar radiation received per unit area (in kilowatt-hours per square meter, kWh/m²) on a horizontal surface. It includes both the direct sunlight and the diffuse sky radiation.​Diffuse Horizontal Irradiation (DIF): Diffuse Horizontal Irradiation is the component of solar radiation received from the sky (excluding the sun's direct rays) on a horizontal surface. It's measured in kilowatt-hours per square meter (kWh/m²).​

* Saudi Solar ChatBot:
This chatbot is designed to provide information and answer queries related to Saudi Arabia's Vision 2030 initiative, with a specific focus on solar and renewable energy projects. The Saudi Solar ChatBot offers users an intuitive interface to inquire about the latest solar initiatives, and the overall progress toward renewable energy targets in Saudi Arabia.

# Methodology: 
* Image Classification: Pre-trained model (MobileNet).
* Object Detection: YoloV8.
* Predicting Generated Energy: Ridge Regressor.
* Location Recommender: K-means Clustring.
* Saudi Solar Chatbot: Large Language Model(LLM): gpt-3.5-turbo, LangChain for localization, OpenAI for natural language processing, and Gradio has been utilized to provide a graphical user interface (GUI) for seamless interaction. 

# Result: 
* Image Classification: accuracy -> 91.66% 
* Object Detection: precision -> 52.7% , recall -> 58.2%
* Predicting Generated Energy: Mean Square Error (MSE) -> 1.08
* Location Recommender: K-means Clustring.
