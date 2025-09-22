SparkSense: Smart Machine Health and Fault Monitoring

SparkSense is an intelligent platform for monitoring and diagnosing industrial electrical machines and rotating equipment, especially focused on factory and shop-floor scenarios found in India. It makes use of modern sensors and machine learning to provide real-time status, early warnings, and actionable recommendations.

What SparkSense Monitors?

The system continuously records and analyzes the following parameters:
Temperature – Prevents overheating and detects changes in environmental or machine heat.
Vibration – Identifies imbalance, bearing damage, mounting issues, and worn or faulty parts before breakdown.
Current – Watches for overload, phase loss, abnormal power draw, and other electrical issues.
Rotational Speed (RPM) – Detects slips, stalls, crashes, and over-speed conditions that typical sensors miss.
Operating Hours – Tracks how long each machine runs, making maintenance scheduling easier.

All sensor data is collected with affordable hardware found in most Indian engineering labs, like DS18B20 (temperature), MPU6050 (vibration), ACS712 (current), hall sensors, and similar devices.

What the Model Does?

SparkSense reads signals from connected machines and:
Cleans and standardizes the raw values.
Detects subtle, unusual patterns using AI-based anomaly detection.
Classifies every major fault—mechanical, electrical, tool wear, power loss, overload, bearing/rotor damage, and more—so that the operator immediately knows the problem.
Warns when any measured parameter is close to a safety or damage threshold long before failure.
Offers clear, direct recommendations for action based on the identified fault, saving valuable diagnostic time.
Works in real time, on low-cost hardware, and sends results wirelessly (using open protocols like MQTT).

Advantages

Suited for Indian industrial equipment and conditions, with 50 Hz defaults and common machine types.
Helps catch issues early—reducing accidents, sudden machine stops, and unexpected repair costs.
Enables maintenance teams to act before a problem becomes a crisis, based on data not guesswork.
Lowers both hardware and operations costs. No expensive PLCs or proprietary solutions required.
Easy to expand: works with single machines, plant-level deployments, or integration with cloud dashboards.
Gives direct, practical advice instead of just raw sensor readings or cryptic error codes.

Datasets and Modeling

SparkSense supports open, industry-relevant datasets such as vibration, current, and temperature records from Indian induction motors and bearings. It also works with internationally recognized sample sets like the AI4I 2020 database. Models are built using Python and scikit-learn, and are easily updated or replaced as new data (or new fault categories) become available.

Getting Started

Download or clone the repository. Place your sensor firmware on ESP32 hardware or use the provided simulation setups. Collect and upload your raw sensor data, then use the provided Python notebooks to train and test your fault detection models. Once satisfied, models can be deployed for live monitoring or further tuning.

Project Organization

Firmware: Microcontroller code for sensor data collection
Model: Data preprocessing, training, and inference scripts
Data: Example datasets with links for benchmarking
Docs: Schematics, explanations, and best practices

This README: Overview and instructions

Contact and Credits

SparkSense is maintained by passionate engineers and students. Special thanks to research and industry contributors, as well as supporters of open-data machine learning in India and globally.

For questions, improvements, or collaboration, feel free to submit issues or pull requests.
