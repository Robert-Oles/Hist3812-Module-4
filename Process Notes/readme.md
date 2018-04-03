# Process Notes #

## April 1 ##

### Resources ###

[Unity](https://unity3d.com/get-unity/download)
[Android Studio](https://developer.android.com/studio/index.html)
[Vufornia](https://www.vuforia.com/)
[Java Development Kit](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

**Step 1**

Begin by downloading Unity, Android Studio, and the Java Development Kit making sure to install packages that are relevent to android development. 

**Step 2**

Find an image that you wish to use as your target image, for this project, the progress target image was created using photoshop's heal brush to replace the black text to text made from bones.

**Step 3**

Go to [Vufornia](https://www.vuforia.com/) and create a free account. Afterwords, create a development license key that we will return to later. Once that is done, go to the target manager and create a new database with your desired target image. 

*important note here: Sicne Unity's default units are meters, you must set the scale of your target image to your desired scale. Since we wanted this to be a landscape piece of paper the scale was set to 0.2794

**Step 4** 

Finalize and download the database you just created for use in Unity.

**Step 5**

Open Unity and create a new project for 3D Development

**Step 6**

Delete the main camera on the left hand side, then under Game Objects > Vuforia click AR Camera

**Step 7**

Click on the AR Camera Hierarchy listing and under inspector click open Vuforia Configuration

**Step 8**

Under App License Key copy and paste the Vuforia License Key that you created earlier

**Step 9**

On your computer, double click the Vuforia Database file that you created earlier and it will import it to you Unity Project

**Step 10**

Back in Unity, under Game Objects > Vuforia click image, which will default to one of the preset ones set by Vuforia

**Step 11**

Click the imagetarget in the Hierarchy listing and under the inspector, change Database to your Vuforia database and Image to your image from that database

**Step 12**

Going back to Vuforia Configuration, under the header Databases, click the check mark for your Vuforia Database and the checkbox beneath it labeled Activate

**Step 13**

Import your model asset to Unity by clicking Assets > Import New Assets

**Step 14**

Drag and drop your model into the scene and using the transform tools, rescale the model and rotate it to work for your intended target

*For this project, the models scale was set to 0.003 with an X rotation of 270 degrees

**Step 15**

Under the hierarchy list drag the asset file onto the imagetarget listing to make it a child of that image target

**Step 16**

Under File > Build Settings click Android and then click Switch Platforms and select Add Open Scenes

**Step 17**

Click Player Settings in the Build Settings menu and change the company and product name to what ever you desire, for example I set the Company name to Robert and the Product name to Robert Oles Progress so that it was easy to find for my Professor. Then under Identifcation change the Package name to something that fits the following format com.companyname.productname for this project I used com.Robert.Robert_Oles_Progress

*Note the use of underscore because the format can't recognize spaces*

**Step 18**

Under Playersettings, scroll to the bottom to XR Settings and enable Vuforia AR Support

**Step 19**

Under Build Settings, Select Build and create your APK File.

**Step 20**

Email or transfer the Apk file to your phone, install and run the application and Voila a brand new AR app

Still need more help? 

[Try this awesome tutorial resource](https://www.youtube.com/watch?v=MtiUx_szKbI) 
