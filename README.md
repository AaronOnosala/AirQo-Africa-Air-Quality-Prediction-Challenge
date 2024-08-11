# AirQo Africa, Air Quality And Pollution Estimation Project

collaboration: [AirQo Africa](https://www.airqo.net/), [Mozilla Foundation](https://foundation.mozilla.org/en/), [Makerere University Artificial Intellegence Lab](https://air.ug/)

<img width="328" alt="Screenshot 2024-08-11 at 18 29 45" src="https://github.com/user-attachments/assets/ef0696bd-92a7-48b0-9990-6744a49dd0c0"> <img width="233" alt="Screenshot 2024-08-11 at 18 29 58" src="https://github.com/user-attachments/assets/8984f882-a2db-48ba-bc37-14e8e120bfe3">

## Background

Air pollution is the world's largest environmental health risk, leading to 7 million premature deaths globally each year, with the most severe impacts felt by poor communities in developing countries. Accurate air quality data is crucial for developing effective interventions to mitigate these risks. In Sub-Saharan Africa, low-cost IoT sensor networks have potential but are expensive to implement and maintain. Satellite-derived PM2.5 estimates based on Aerosol Optical Depth (AOD) and machine learning techniques offer a scalable solution to estimate pollution levels over large areas. This approach can support the development of vulnerability risk profiles, health preservation strategies, environmental protection measures, community empowerment, and climate change mitigation.

## Problem Statement

The project aimed to estimate PM2.5 levels from satellite observations based on AOD for eight cities in seven African countries: Lagos, Accra, Nairobi, Yaoundé, Bujumbura, Kisumu, Kampala, and Gulu. The challenge was to develop a machine learning model that could accurately estimate PM2.5 levels, which would then be validated using ground-based observations.

## Approach

To tackle this challenge, we utilized several machine learning models, ultimately finding that the TensorFlow Decision Forest model was the most suitable for this specific task. The models were trained using a dataset of satellite-derived AOD and corresponding PM2.5 ground observations from the selected cities.

## AI Methods Applied
 1. __Data Collection and Preprocessing:__

Collected satellite-derived AOD data and corresponding PM2.5 ground observations for the eight cities. Cleaned and preprocessed the data to ensure consistency and accuracy. 

 2. __Model Selection:__

Evaluated multiple machine learning models, including linear regression, random forests, and neural networks. Selected the TensorFlow Decision Forest model for its superior performance in handling structured data and capturing complex relationships between features.

 3. __Training and Validation:__

Employed the leave-one-out cross-validation technique to train the model, a resource-intensive but robust method for small datasets. This technique involves training the model on all cities except one and then validating it on the excluded city, repeating this process for each city.

## Challenges Faced

 * __Data Quality:__ Ensuring the quality and consistency of the satellite-derived AOD data and ground observations.

 * __Model Complexity:__ Balancing model complexity and computational efficiency, especially with the leave-one-out cross-validation technique.

 * __Resource Constraints:__ Managing limited computational resources while training and validating multiple models.

## Outcomes

The TensorFlow Decision Forest model achieved a Root Mean Squared Error (RMSE) of 17.69, indicating high accuracy in estimating PM2.5 levels. This performance demonstrates the model's effectiveness in capturing the relationship between AOD and PM2.5, making it a valuable tool for air quality estimation in African cities. The models developed in this project will be deployed through [AirQo's digital platform here,](https://www.airqo.net/) empowering communities with access to crucial air quality information. This data will provide the evidence needed to tackle local pollution challenges, improve public health, and achieve environmental justice.

## Quantified Success

 - __Model Performance:__ Achieved an RMSE of 17.69, indicating high accuracy.
 - __Community Impact:__ Enabled the development of targeted interventions for air quality improvement and public health protection.
This project showcases the application of advanced machine learning techniques to address a significant environmental health challenge, highlighting the potential of AI in driving positive societal impacts.

## Conclusion
The Air Pollution Prediction project successfully leveraged advanced machine learning techniques to estimate PM2.5 levels from satellite-derived Aerosol Optical Depth (AOD) data for eight cities in seven African countries. The project demonstrated that the TensorFlow Decision Forest model is highly effective in predicting air pollution levels, achieving an RMSE of 17.69 with leave-one-out cross-validation. This level of accuracy signifies the model's capability in capturing the complex relationship between AOD and PM2.5.

By providing a scalable and cost-effective solution for air quality estimation, this project addresses critical gaps in air pollution data in Sub-Saharan Africa. The accurate PM2.5 predictions enable the development of vulnerability risk profiles, health preservation strategies, and environmental protection measures. Furthermore, the integration of these models into AirQo's digital platform empowers communities with actionable data, fostering informed decision-making and advocacy for environmental justice.

The project also highlights the potential of AI and machine learning in tackling significant environmental health challenges, showcasing their applicability in diverse settings with limited resources. Overcoming challenges related to data quality, model complexity, and resource constraints, the project underscores the importance of innovative approaches and rigorous validation techniques in achieving reliable and impactful outcomes.

In conclusion, the Air Pollution Prediction project not only advances the field of environmental data science but also contributes to the broader goal of improving public health and environmental sustainability in Africa. Through continued collaboration and technological innovation, such initiatives can drive significant progress in addressing the global air pollution crisis.
