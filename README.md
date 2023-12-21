### 2023_KSW_Fall_Program

### Team HoT

## Project Title

Establishing the Correlation Between Bio-Data and Concentration Level Utilizing EEG Data

## Project Period
 Sep/20/2023 ~ Dec/20/2022 

## Project Content
1. [Collaborator](#collaborator)
2. [Project Overview](#project-overview) 
3. [Research problem statements](#research-problem-statements)
4. [Research novelty](#research-novelty)
5. [Environment Setting](#environment-setting)
6. [Experiment](#experiment)
   <!--   - [File Structure](#file-structure)
    - [Dataset](#dataset)
    - [Requirments](#requirments) -->
   <!--
    - [Result](#result)     
    - [Model Architecture](#mode-architecture) -->

## Team Members

| Name         | University               | Department                                   | Email               | Contact                        |
| :------------- | :------------------------: | :--------------------------------------------: | :-------------------: | :------------------------------: |
| Seojeong Park    | Hallym University        | Computer Science                    | diditjwjd@gmail.com | https://github.com/seojeongP     |
| Seungah Jang  | Jeju National University        | Computer Science                    | wkdtmddk6733@gmail.com   | https://github.com/ssaaJang     |
| Jeongmin Seo | Kyunhee University     | Computer Information                | balljm@naver.com | https://github.com/jeongmin1217       |
| Yunhui Lim | Kyunhee University     | Computer Science and Engineering                | lyhhh0320@gmail.com   | https://github.com/YunheeLim    |
| Byeongsoo Min  | Kyunhee University | Computer Science and Engineering       | qud9783@gmail.com   | https://github.com/Byeongsoo-Min  |
| Martin Kim | Purdue University        | Computer Science | 19alswprla@gmail.com    | https://github.com/19alswprla |


## Project Overview
<p align="center">
<img width="1000" alt="architecture" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/9032607c-dc88-4661-8c5c-600f3c55e6b4">   
</p>

>### Machine Learning Process
<p align="center">
<img width="700" alt="architecture" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/dd04f249-a38f-4e9f-88ce-a8f5615ad139">   
</p>

>### Service Architecture
<p align="center">
<img width="500" alt="architecture" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/940893d5-319f-4e06-b7a2-1deb2c91f46e">   
</p>

## Research Problem Statements 

Modern day society has bore witness to a phenomenon of diminished concentration levels and attention spans as a result of dependency and increased usage of smart phones. The usage rate of smartphones is more than 70% of adults in the United States and nearly 50% of adults worldwide. The decline in cognitive ability in daily life due to the increase in smartphone use can be observed. Therefore, the need for methods to facilitate and assist users in maintaining high levels of concentration in their daily lives has increased significantly.

## Research Novelty 
1. This study adopted a wearable device in daily life to measure the concentration level instead of using a specialized EEG sensor.<br>
2. This study set the experimental background as a everyday life.<br>
3. Extracted brainwaves were used as a direct indicator of concentration without Fourier transform.<br>
4. A quantified figure was utilized to analyze a concentration score instead of subjective self-assessment.<br>
5. The correlation between bio-data and concentration is provided with importance and proportionality.
   
## Environment Setting
>### Machine Learning

>### Service
1. Go to https://nodejs.org/en and download Node.js
2. Download the Expo Go app on your phone in App Store or Google Play Store.
3. Follow the command below in your bash.
```bash
npm install --g expo-cli
```
```bash
git clone 
```
```bash
npm start
```
4. Scan the QR code that can be shown in the console with your phone.
<p align="center">
<img width="200" alt="app_screen1" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/7922116d-d626-4ee6-8557-abb10b9c63b6"> 
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
<img width="200" alt="app_screen2" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/435d4f48-ec10-4fb7-82b8-cb929072e45b">
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
<img width="200" alt="app_screen3" src="https://github.com/Healthcare-of-Things/CandY-front/assets/92131041/dfa05cae-f907-47e8-950d-d0d672b6820d">    
</p>

#### Requirements
```
- npm version 8.1.0
- expo-cli version 6.3.10
```

## File Structure
    📦2023-ksw-fall-program-final-team-hot/
     └📂presentation
      └📜Mid-Presentation-Team-HoT.pptx
      └📜Final-Presentation-Team-Hot.pptx
      └📜demo.mp4
     └📂paper
      └📜paper.pdf
     └📂code
       └📂data_analysis
       └📂frontend
         └📂assets
         └📂components
           └📜CircleProgress.js
           └📜CircularProgress.js
         └📂node_modules
         └📂screens
           └📂Home
             └📜Bluetooth.js
             └📜Home.js
           └📂Main
             └📜Main.js
           └📂OnBoarding
             └📜LaunchScreen.js
             └📜SignInScreen.js
             └📜SignUpScreen.js
           └📂Profile
             └📜Profile.js
           └📂Recommendation
             └📜Recommendation.js
           └📂Record
             └📜Record.js
           └📂Statistics
             └📜DailyStatistics.js
             └📜SessionStatistics.js
             └📜Statistics.js

         └📜App.js
         └📜app.json
         └📜babel.coonfig.js
         └📜package-lock.json
         └📜package.json
         └📜react-native.config.js
         └📜yarn.lock
       └📂backend
     └📜README.md
       

## Experiment
    
>#### Result

#### k=5

|   |R2|RMSE|MAE|
|---|:-:|:-:|:-:
|**Extra Tree Regressor**|0.8600|0.0902|0.0609|
|**Optimized ETR**|0.8610|0.0899|0.0608|
|**RandomForest Regressor**|0.8286|0.0998|0.0680|
|**Optimized RFR**|0.8316|0.0989|0.0674|
|**XGBoost Regressor**|0.7979|0.1084|0.0780|
|**Optimized XGBR**|0.8270|0.1003|0.0701|

#### k=10
|   |R2|RMSE|MAE|
|---|:-:|:-:|:-:
|**Extra Tree Regressor**|0.8745|0.0854|0.0579|
|**Optimized ETR**|<span style="color:red">0.8763</span>|0.0848|0.0576|
|**RandomForest Regressor**|0.8430|0.0955|0.0652|
|**Optimized RFR**|0.8444|0.0951|0.0649|
|**XGBoost Regressor**|0.7993|0.1084|0.0774|
|**Optimized XGBR**|0.8314|0.0990|0.0689|
