# Bee Guardian 2.0

**A Smart Beehive Health Monitoring System Using an Embedded Multimodal System**
Final Year Project, BS Computer Science, Namal University Mianwali

## Overview
Hive inspection in Pakistan is mostly manual, so problems such as mite infestation or a missing queen are often noticed late.
Bee Guardian 2.0 monitors a hive automatically using sound, images and sensor data (temperature, humidity, weight and entrance traffic). The data is sent to a server, where AI models analyse it and a fusion model combines the results into one health score. The beekeeper sees the score and alerts in a mobile app.

## Project Work
1. **Hive unit:** a hive-mounted unit with a camera, microphone, temperature/humidity sensor, weight sensor and entrance traffic sensor, controlled by an ESP8266. It captures data every 15-30 minutes and uploads it over Wi-Fi.
2. **Dataset collection:** collecting and labelling audio, image and sensor data from the hive.
3. **Sound analysis:** an audio model that detects signs such as queenlessness or colony stress.
4. **Image analysis:** an image model that detects visible problems such as mites and damaged wings.
5. **Sensor analysis:** a model that checks temperature, humidity, weight and bee-traffic trends.
6. **Fusion model:** combines all the results into one health score.
7. **Backend server:** receives the data, runs the models, stores the hive history and triggers alerts.
8. **Mobile app:** shows the health score, hive history and alerts to the beekeeper.
9. **Testing and evaluation:** running the complete system on a live hive and measuring its accuracy and reliability.

## How It Works
1. The hive unit reads its sensors and uploads data over Wi-Fi every 15-30 minutes.
2. The server runs the sound, image, sensor and traffic models.
3. The fusion model produces one health score.
4. The mobile app shows the score, history and alerts.


## Planned Hardware (hive unit)
ESP8266 (NodeMCU ESP-12E), ArduCAM Mini 2MP (OV2640) camera, MAX4466 microphone, DHT22 temperature/humidity sensor, HX711 with load cells (weight), IR break-beam sensor (entrance traffic), microSD module.
The full list is in `Hardware/`.

## Repository Contents
- `Proposal/` : project proposal
- `Presentations/` : defense presentations
- `Architecture/` : system and embedded architecture diagrams
- `Research/` : dataset research
- `Hardware/` : component list and hardware requirements

Source code (firmware, models, backend, app) will be added as the project progresses. Raw datasets are not stored in this repository.

## Team
- Huzaira Sultan (NUM-BSCS-2023-07)
- Aiman Malik (NUM-BSCS-2023-26)

Supervisor: Dr. Shafiq-ur-Rehman
Co-supervisor: Mr. Muhammad Bilal
