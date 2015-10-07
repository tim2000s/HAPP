# HAPP ~ Hackabetes Artificial Pancreas Project

Native Android implentaion of the OpenAPS.org algorithm with addiotnbal funcatiniality.

Current features:
* Capture your Bolus and Carb Treatments
* Bolus Wizard
* Suggested Temp Basal based on OpenAPS.org algorithm
* Notifications for Android and Android Wear when a new Temp Basal is suggested
* Visuals showing Carb and IOB over time and Basal vs Temp Basal adjustments

As of now the App can be used to infom the user at a user set time interval suggested Temp Basal as caculated by the OpenAPS.org algorithm, this can then be manually set on the users pump.
This allows a Diabetic with any pump to experiment with the OpenAPS algorithm.

Requirements:
* xDrip device and App for capturing blood sugar values
* Android 5.0

### Whats next?
To integrate with the Roche Accu-Chek Combo pump. Any experience hacking Bluetooth? Please contact me.

### Why would I be interested?
As you can now play with the OpenAPS algorithm with any pump :)

### Common questions
* Q: Why have you not focused on the current Round Trip Android app?
* A: This was ported from the native Java implementation of OpenAPS to Android by a hired developer along with all Medtronic integration. I wanted a ground up native port of the OpenAPS system, by doing it myself I can learn as much as possible and be sure I am porting over only the items I require.
* Q: Why are you not reading Treatment Data from the pump
* A: I am building the system to support the Roche pumps where Treatment data is captured on the Bluetooth enabled Blood Meter. This App is a complete replacement of this meter that will I hope link to the pump via Bluetooth.
* Q: Why do you not use the native OpenAPS Java files?
* A: I hear this is possible on Android, but believe this would be difficult to debug. One aim of this project is to provide an easy to debug version of determine_basal to help me understand the OpenAPS algorithm
* Q: Why have you done X and not Y in Android
* A: I am not a developer and have been only working on Android development for the last 2 months, if there is a better way to do something please do let me know

###To do
* Fix UI bug in line charts where lines appear to loop back on themselves
* Write up the core functions of the App
* Improve code comments
* Lots and lots of debugging
* Find a Bluetooth developer to help me hack the Roche Accu-Chek Combo pump
