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
Make sure to follow all the following steps:  

1. Creating a game in the facebook UI:    
[https://developers.facebook.com/apps](https://developers.facebook.com/apps)  

2. Create an app:
   The following manula by Meta is explaning how to create an app.
   [https://developers.facebook.com/docs/development/create-an-app/](https://developers.facebook.com/docs/development/create-an-app/)  
   When you need to choose they type of the app, choose the Other > Gaming app. 

3. Go to Settings > Basic and fill the needed info

4. Create a valid privacy policy and User data deletion:
   Create Privacy policy on: [https://app-privacy-policy-generator.firebaseapp.com/](https://app-privacy-policy-generator.firebaseapp.com/)
   After creating, downloading it and opening it on Google Docs. 
   Under "File" choose "Publish to the web" and it will create you a Privacy Policy link.
   Insert the created link on Both privacy policy and User data deletion sections, and choose the needed Category and Sub-Category.
   ![Basic](images/facebookBasic.png)
5. Choose and add your platform: 
   Android fill the package name (it’s the bundle), and on IOS fill App’s ID and Bundle ID.
6. Other sections or to confirm ownership are not mandatory so don’t worry about it!
* Click “Save Changes”

7. Add Moonee’s Ad Account ID

For us to be able to test your game, we need to connect it to our Ad Account:
Go to Settings -> Advanced and fill the needed info:
Scroll down to the section “Advertising Accounts” and insert:
267507499172466

8. Activate your app. 
Make sure to set the status on the first row to”Live”
Click Save

Step 6: Verify data
You can download + open the app, and check on FB Developer main dashboard, if you’re seeing data of last date installs:



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

- For Android: 
Please make sure your app’s privacy and security practices match the store’s standards.   
[link](https://docs.google.com/document/d/1xN6lX-wWwJfFPhiAr2oifMPD_mAtMWC39qZdFRv2uFY/edit)
**Policy Declaration for Play Safety Label Android**

You need to fill this part in Google Play store as the following: 

APP CONTENT -> DATA SAFETY -> DEVICE OR OTHER IDENTIFIERS.

- For IOS:
Please make sure your app’s privacy and security practices match the store’s standards. 
Use this how-to guide.

## 6. Ready For Testing

1. Once you finish all of the above steps and your game is good to go, publish it on Google Play Store/ App Store.
2. Once the game is live, share in the Slack Channel the game’s store URL and its Facebook App ID.
3. Make sure you’ve done all the needed steps here:
Meta Instructions For Testing.

