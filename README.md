&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![LOGO](images/logo.png) 

# Welcome to MOONEE’s family! 🚀
### We've Been Expecting You!
Welcome aboard! Whether you're a seasoned developer or just starting out, this guide is tailored to help you navigate your journey within our developer community. Here, you'll find instructions, guidelines, and solutions to your technical inquiries.

Don't hesitate to reach out to us with any questions or requests for further information. We're here to support you and your team every step of the way, from prototyping to testing. Before committing extensive resources, we aim to gauge your app's potential in terms of retention, CPI, playtime, and other key performance indicators (KPIs).

Our test will target US users and will conclude within a maximum of 4 days, providing invaluable insights into your app's potential.

Remember, at MOONEE, data is paramount. It's the cornerstone of our decision-making process. We look forward to collaborating with you and leveraging data to drive success!

# Prototype Test Instructions

<details>
  <summary>Table of Contents</summary>
  
  1. [System Requirements](#system-requirements)
  2. [Platform Settings](#platform-settings)  
    A. [Facebook](#facebook)  
    B. [Game Analytics](#game-analytics)  
  5. [Video Creatives](#video-creatives)
  6. [SDK Implementation](#sdk-implementation)
  7. [Commen Issues](#commen-issues)
  8. [In-Game Fonts](#in-game-fonts)
  9. [DATA Safety](#data-safety)  
      A. [Android](#android)  
      B. [iOS](#ios)
  10. [Ready For Testing](#ready-for-testing)
</details>

## System Requirements
<details>
  <summary></summary>
  
  - Unity Editor 2021.2 or higher (2021 LTS version)
  - Android:
    - Minimum SDK: Lollipop 5.0 (API 22)
    - Scripting backend: IL2CPP
  - iOS:
    - Target minimum iOS Version: 13.0
    - Scripting backend: IL2CPP
</details>

## Platform Settings
<details>
  <summary></summary>
  It’s not mandatory for the game to be live yet in the store for this part.

  ### Facebook
  <details>
    <summary>Expand</summary>

#### 1: Creating a game in the [Facebook UI](https://developers.facebook.com/apps)

#### 2: Create an app

The following manual by Meta explains how to create an app: [Manual](https://developers.facebook.com/docs/development/create-an-app/)

When you need to choose the type of the app, choose "Other" > "Gaming app".

#### 3: Go to Settings > Basic and fill the needed info

#### 4: Create a valid privacy policy and User data deletion

  A. Create Privacy policy on: [this link](https://app-privacy-policy-generator.firebaseapp.com/)  
  B. After creating, download it and open it on Google Docs.  
  C. Under "File" choose "Publish to the web" and it will create you a Privacy Policy link.  
  D. Insert the created link on Both privacy policy and User data deletion sections, and choose the needed Category and Sub-Category (Hyper Casual, Hybrid etc.).
![Basic](images/facebookBasic.png)
#### 5: Choose and add your platform

  A. Android: fill the package name (it’s the bundle), and on iOS fill App’s ID and Bundle ID.  
  B. Other sections or to confirm ownership are not mandatory so don’t worry about it!  
  C. Click “Save Changes”.
  ![Android](images/Android.png)

#### 6: Activate your app

Make sure to set the status on the first row to "Live".
![live app](images/liveAppMeta.png)

#### 7: Add Moonee’s Ad Account ID

For us to be able to test your game, we need to connect it to our Ad Account:  
  a. Go to Settings -> Advanced and fill the needed info:  
  b. Scroll down to the section “Advertising Accounts” and insert Moonee’s Ad Account ID:`267507499172466`.
![account](images/AccountID.png)
#### 8: Verify data

You can download + open the app and check on FB Developer main dashboard if you’re seeing data of last date installs.

#### 9: Share in the Slack channel your FB App ID.

  </details>

  ### Game Analytics
  <details>
    <summary>Expand</summary>  

1. Create a Game analytics account and asset using this [link](https://tool.gameanalytics.com/login?redirect=%252F).
2. If your game is level-based, make sure to have the events:
   - Start
   - Complete
   - Fail
3. Make sure to have the level events naming in the format:
   - “Level0001”
   - “Level0002”
   (Make sure to start from level 0001 and not from 0000)
4. Grant us Admin access to the app on Game Analytics: 
   - Settings -> Users -> Invite users -> for this user erez@moonee.io
  </details>
</details>

## Video Creatives
<details>
  <summary></summary>
  
1. Provide gameplay videos for ads (preferred via Google Drive) with game sounds (if there are ones).
2. Two videos are needed in a format of 1080x1350:
   A. Length of 2 minutes of different fails.
   B. Length of 3 minutes which include normal play, expert play, and satisfying moments (Unique scenes and highlights of the game).
3. Recording tips:
   - Please use the official Unity package called “Unity Recorder”. This package allows you to capture footage directly from the engine in all of the required resolutions, without any need for external software. You can install it from the package manager under the Unity Registry packages.
   - Once installed you can access it here (Window > General > Recorder > Recorder Window):
     ![recorderWindow](images/recorderWindow.png)
     ![recorderWindow](images/record.png)
   - Click “Add Recorder” - make sure you add a Movie Sequence and remove the Image Sequence if there is one.
   - Source - Game View
   - Switch target fps to 60/30.
   - Make sure to change the output resolution to “Custom”. Change to the desired resolution (W1080xH1350) and record from the game view.
   - Press “Start Recording”, the game should start and the engine will record.
   - Reach your new captured footage file from the selected folder.
   - For further information regarding the tool, see the official unity guide: [About Unity Recorder](https://docs.unity3d.com/Packages/com.unity.recorder@3.0/manual/index.html).
</details>


## SDK Implementation
<details>
  <summary></summary>  
**Please remove all other SDK’s before implementing Moon SDK!**  

   1. Downloading the MOON SDK   
The current version of the MOON SDK is version 1.3.5  (link is sent by slack bot)  
**Notice: For this test use only Facebook, Game analytics and Adjust SDKs features!**
  2. Setting Up Moon SDK:

  3. Import MoonSDK.unitypackage into your unity project.
  
  4. The MoonSDKScene must be the first in the list in the build settings, after initialization it will load the next scene in the list (with index 1).

     ![MoonSDKScene](images/MooneeScene.png)
     
  5. Open MoonSDK settings and fill in all app keys for analytics and advertising services which you want to use and press Check and Sync Settings button
    
     ![SyncSettings](images/SyncSettings.png)
 
 6. Initialization: Moon SDK is initialized automatically from the Moon SDK scene.

 7. Progression Events:
    
**Levels progression events using Adjust and Moonee's Developer's Dahboard:**

      MoonSDK.SendLevelDataStartEvent((GameModel.levelIndex + 1).ToString());  
      MoonSDK.SendLevelDataCompleteEvent(LevelStatus.complete, (GameModel.levelIndex + 1).ToString(), LevelResult.win, isContinueLevel); 


LevelDataCompleteEvent has a few arguments:
  1. **LevelStatus** - Indicates the current status of the level, which could be "start" when the level begins, "fail" if the player fails to complete it, or "complete" if the player finishes it without winning.
  2. **LevelResult** - Represents the outcome of the level, which could be "win" if the player successfully completes it or "fail" if the player fails to complete it.
  3. **isContinueLevel** - A boolean argument that indicates whether the player is continuing the level from where they left off (true) or starting it from the beginning (false). This is particularly useful for long idle levels or when there's a revive   
     option. If the game doesn't have these features, it should be set to false by default.


**Levels progression events using GameAnalytics:**  

      void MoonSDK.TrackLevelEvents(MoonSDK.LevelEvents eventType, int levelIndex);
      MoonSDK.TrackLevelEvents(MoonSDK.LevelEvents.Start, 1);

 8. Make sure you filled the mandatory keys for the test under Facebook, Game Analytics and Adjust Basics section
You will get the needed Adjust tokens from your Publisher Manager

</details>

## Commen Issues
<details>
  <summary></summary>  
Commen issues can be found here as well as in the "issue" section.
Please add your comments there as well, to allow other to gain from it.

**Importnat comments:**
1. Please remove External Dependency manager folder from the project and import the latest one.
   
</details>

## In-Game Fonts
<details>
  <summary></summary>  
In terms of in-game fonts, they must be official fonts from Google Fonts or Liberation Sans from Unity. Follow these steps to ensure compliance with font licensing:

1. Use only fonts from the Google Fonts library or Liberation Sans from Unity.
2. After selecting the relevant font, ensure you have the license for the game code as a text file.
3. Rename the license file to the following format: `Fontname_license.txt`.
4. Place both the font file and its license file in the Fonts directory of your project.
5. The most common font licenses are OFL (Open Font License) and Apache License.
6. Copy everything in the StreamingAssets directory to add a new licensed font, which will be automatically added to the build.
7. Fonts from Google Fonts can be used for both Android and iOS games. You can find them at [Google Fonts](https://fonts.google.com/).
8. Unity typically has two built-in fonts:
   * Liberation Sans (free to use)
   * Arial (note: Arial is not free to use)
9. Refer to the following guides for embedding custom fonts in games:
   * Unity - Manual: [Font Assets](https://docs.unity3d.com/Manual/class-Font.html).

By adhering to these guidelines, you ensure that your game uses licensed fonts responsibly and legally.

</details>

## DATA Safety
<details>
  <summary></summary>

### Android
<details>
  <summary></summary>
To complete the Data Safety form required by the Google Store, please adhere to the following steps:

Access the Google Play Console for your application.
Navigate to the "Data safety" section within the console.
Answer the questions as below:  

**Overview:**  
Please read the following instructions carefully to ensure that you are not collecting data beyond the parameters outlined below. If, however, you find that you are inadvertently collecting additional data, please promptly contact us for further assistance. It is essential to adhere strictly to the specified data collection guidelines to maintain compliance and transparency with our policies.  

**Data collection and security:**  
Does your app collect or share any of the required user data types? _Yes_
  - Is all of the user data collected by your app encrypted in transit? _Yes_
  - Which of the following methods of account creation does your app support? _My app does not allow users to create an account_
  - Do you provide a way for users to request that their data is deleted? (Optional) _No_ 

**Data types:**  
Select all of the user data types collected or shared by your app.
- Location: _None_
- Personal info: _None_
- Financial info: _None_
- Health and fitness: _None_
- Messages: _None_
- Photos and videos: _None_
- Audio files: _None_
- Files and docs: _None_
- Calendar: _None_
- Contacts: _None_
- App activity: App interactions (Information about how a user interacts with your app. For example, the number of times they visit a page, or what they tap on.)
- Web browsing: _None_
- App info and performance: Crash logs
- Device or other IDs: Device or other IDs

**Data usage and handling** _Manage in the errow for both types:_

App Activity / App interactions:
  - Is this data collected, shared, or both? _Collected_
  - Is this data processed ephemerally? _Yes, this collected data is processed ephemerally_
  - Is this data required for your app, or can users choose whether it's collected? _Data collection is required_
  - Why is this user data collected? App functionality, Analytics, Advertising or marketing

Device or other IDs:
  - Is this data collected, shared, or both? _Collected_
  - Is this data processed ephemerally? _Yes, this collected data is processed ephemerally_
  - Is this data required for your app, or can users choose whether it's collected? _Data collection is required_
  - Why is this user data collected? _App functionality, Analytics, Advertising or marketing_
    
**Preview:**  
See that all of the above is correct, and press save.
If you can't see the save button, there are 3dots there, that "save" is one othe options in them.

</details>


### iOS
<details>
  <summary></summary>
To complete the Data Safety form required by the App Store, please adhere to the following steps:

Access the App Play Connect for your application.
Navigate to the "App Privacy" section within the console.
Answer the questions as below:  

**Privacy Policy**  
User Privacy Choices URL: Please provide Moonne's URL: https://moonee.io/privacy-policy/

**Data Collection**  
Do you or your third-party partners collect data from this app? _Yes, we collect data from this app_

**Data Types**  
- Contact Info: _None_
- Health & Fitness: _None_
- Financial Info: _None_
- Location: _None_
- Sensitive Info: _None_
- Contacts: _None_
- User Content: _None_
- Browsing History: _None_
- Search History: _None_
- Identifiers: _Device ID_
- Usage Data: _Product Interaction,Advertising Data_
- Diagnostics: _Crash Data, Performance Data_
- Surroundings: _None_
- Body: _None_
- Other Data: _None_


Identifiers/ Device ID:
- Indicate how device IDs collected from this app are being used by you or your third-party partners? _Third-Party Advertising,Developer’s Advertising or Marketing_
- Are the device IDs collected from this app linked to the user’s identity? _No, device IDs collected from this app are not linked to the user’s identity_
- Do you or your third-party partners use device IDs for tracking purposes? _Yes, we use device IDs for tracking purposes_

Usage Data/ Product Interaction:
- Indicate how Product Interaction collected from this app are being used by you or your third-party partners? _Third-Party Advertising, Developer’s Advertising or Marketing, Analytics,Product Personalization, App Functionality_
- Are the Product Interaction data collected from this app linked to the user’s identity? _No, Product Interaction data collected from this app are not linked to the user’s identity_
- Do you or your third-party partners use device IDs for tracking purposes? _Yes, we use device IDs for tracking purposes_

Usage Data/ Advertising Data:
- Indicate how Advertising Data collected from this app are being used by you or your third-party partners? _Third-Party Advertising,Developer’s Advertising or Marketing, Analytics,Product Personalization, App Functionality_
- Are the Advertising Data collected from this app linked to the user’s identity? _No, Advertising Data collected from this app are not linked to the user’s identity_
- Do you or your third-party partners use Advertising Data for tracking purposes? _Yes, we use Advertising Data for tracking purposes_

Diagnostics/ Crash Data:
- Indicate how crash data collected from this app are being used by you or your third-party partners? _Developer’s Advertising or Marketing, Analytics_
- Are the crash data collected from this app linked to the user’s identity? _No, crash data collected from this app are not linked to the user’s identity_
- Do you or your third-party partners use crash data for tracking purposes? _Yes, we use crash data for tracking purposes_

Diagnostics/ Performance Data:
- Indicate how performance data collected from this app are being used by you or your third-party partners? _Third-Party Advertising, Developer’s Advertising or Marketing, Analytics,Product Personalization, App Functionality_
- Are the performance data collected from this app linked to the user’s identity? _No, performance data collected from this app are not linked to the user’s identity_
- Do you or your third-party partners use performance data for tracking purposes? _Yes, we use performance data for tracking purposes_

</details>  
</details>

## Ready For Testing
<details>
  <summary></summary>
  
1. Once you finish all of the above steps and your game is good to go, publish it on Google Play Store/ App Store.
2. Once the game is live, share in the Slack Channel the game’s store URL and its Facebook App ID.
3. Make sure you’ve done all the steps above
4. Get check for the following:
  - We are getting installs data from the app
  - We get levelDataStrat and levelDataComplete events from the app
</details>

# Good Luck! 

