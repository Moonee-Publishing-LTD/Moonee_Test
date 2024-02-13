# Welcome to MOONEE’s family!
### We’ve been expecting you.


This guide is specially designed for new entrants to our developer community. It should provide you with instructions on how to, guidelines, and answers to your technical questions. 


Please feel free to contact us with any questions, to request further information about any issue or guidance you or your team might need, we will be guiding you and your studio through the whole process of releasing your prototype for testing. Before going with large resources, we want to test the potential of your app in terms of retention, CPI, Playtime and additional KPI’s. The test will be targeting US users and will take us Max 4 days to determine KPI’s.

The KPI’s will determine the game’s potential and provide critical DATA. 
DATA is MOONEE’s key for decision making. 

# Prototype Test Instructions: 
**Please remove all other SDK’s before implementing Moon SDK!**
#

# Prototype Test Instructions
1. System Requirements
2. Platforms Settings
3. Video Creatives
4. SDK Implementation
5. DATA Safety
6. Ready For Testing

## 1. System Requirements
- Unity Editor 2021.2 or higher 2021 LTS version
- Android:
  Minimum SDK: Lollipop 5.0 (API 22)  
  Scripting backend: IL2CPP
- iOS: 
  Target minimum iOS Version: 13.0   
  Scripting backend: IL2CPP
  
## 2. Platforms Settings
It’s Not mandatory for the game to be live yet in the store for this part  
### Facebook
Make sure to follow all the steps in this guide.
Afterwards share in the Slack channel your FB App ID.
### Game Analytics 
1. Create a Game analytics account and asset using this link.
2. If your game is level based, make sure to have the events:
    - Start
    - Complete
    - Fail
3. Make sure to have the level events naming in the format:
    - “Level0001”
    - “Level0002”
- Make sure to start from level 0001 and not from 0000
4. Grant us Admin access to the app on Game Analytics: 
    - Settings -> Users -> Invite users -> for this user erez@moonee.io

## 3. Video Creatives
Provide gameplay videos for ads (preferred via Google Drive) with game sounds (if there are ones)

Two videos are needed in a Format of 1080X1350:
1. Length of 2 minutes of different fails.
2. Length of 3 minutes which include normal play, expert play and satisfying moments (Unique scenes and highlights of the game).
[Recording tips](https://docs.google.com/document/d/1TSD_arNmRhkE10pNvNlMuq6hC8kP0ORHvDvll83p9HU/edit)

## 4. SDK Implementation
Please remove all other SDK’s before implementing Moonlight SDK
The letest SDK version is 1.3.5
Notice: For this test use only Facebook, Game analytics and Adjust SDKs features.

## 5. DATA Safety
## 6. Ready For Testing

