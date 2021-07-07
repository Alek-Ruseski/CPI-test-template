# CPI-test-template
This is a template project for CPI tests (apps that dont have actual gameplay but simply use videos, or are completely empty)

Steps for making a new CPI test:
1. Load new config.
2. Change name of app in Player settings (Product Name)
3. Add a new alias to the keystore.
4. Depending on whether you are building an empty app or video app:
  4.1. (if you have video) Replace the video in the VideoPlayer component of Video object that is a child of the Canvas object.
    - (video is meant to be in the format of 1024x1280 because that's how canvas is set up)
  4.2 (in the case of empty app) add only EmptyScene to scenes in build.
5. Build .apk, send to QA for checkup, and after it's confirmed that AppsFlyer is good then build .aab as well
6. Profit.
