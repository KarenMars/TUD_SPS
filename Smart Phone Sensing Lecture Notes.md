# Smart Phone Sensing Lecture Notes

## Resources

- [Android Development Tutorial Website](<https://www.tutorialspoint.com/android/android_user_interface_layouts.htm>)
- 

## Setting Up Working Environment 

- Gradle-based build system

  what is Gradle-based build system: designed for multi-project builds, which can grow to be quite large. and it supports incremental builds by intelligently determining which parts of the builds tree are up to date; any task dependent only on those parts does not need to be re-executed (from wikipedia) 

- [The Project Structure](<https://developer.android.com/studio/intro>)

  - manifests: contains the AndroidManifest.xml file
  - java: contains the Java source code files, including JUnit test code
  - res: Contains all non-code resources, such as XML layouts, UI Strings, and bitmap images

## Notes for Tutorials 

- 中文 [link](<https://developer.android.com/guide/components/activities/intro-activities?hl=zh-cn>)
- How to access the resources in Android
- Activities in Android 

### Build the first app

- Two concept  to be known before building the first APP
  - APPs provide multiple entry points
  - APPs adapt to different devices  

- Changing the phone into developer mode 

  Find the build number on the phone (版本号) and tap on it seven times and the phone is under the development mode. 


##  Lecture 1 Logistics of the Course

### Task Description

- Scenario: indoor localization 

  (GPS cannot perform indoor localization due to the signal cannot penetrate the building materials)

- Sensors: internal sensors and external sensors 

- Methods: Signal processing methods, Machine learning methods ......

- Overall time line: 

  KNN -> week3 -> 10%

  Bayes Filters -> week6 -> 10%

  Particle Filters -> week 8 -> 80%

### KNN & RSSI for Activity Monitoring and Localization

- RSSI (Received signal strength indication)

  RSSI is the relative received signal strength in a wireless environment, in arbitrary units. RSSI is an indication of the power level being received by the receiving radio after the antenna and possible cable loss. The greater the RSSI value, the stronger the signal. RSSI is represented in a negative form, the closer value is to 0, the stronger the received signal has been. 

- Steps for classification

  - raw signal (directly obtained from sensors)

  - feature extraction 

    *How to select features?*

    - Mean
    - Variance
    - Max Min
    - Fourier transform
    - autocorrelation 

  - classification methods 

    **KNN** -> How to choose an appropriate K 

    ​	  -> Different kinds of distances: Euclidean/Manhattan/Hamming/Mahalanobis 