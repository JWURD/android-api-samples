# WRLD Android Java API Samples
Samples demonstrating how to use the [WRLD Android Java Api](https://docs.wrld3d.com/android/latest/docs/api/) to display beautiful, interactive 3D maps on Android devices.

## Building and running the samples
### Prerequisites
* [Android Studio](https://developer.android.com/studio/index.html), together with the Android SDK and supporting libraries appropriate for your target platform.
* For running on Android devices, the library requires Android 4.0.3 (API level 15) or higher.

### Setup
* Clone or downloaded snapshot of this repo.
* Obtain a [WRLD API key](https://www.wrld3d.com/developers/apikeys/). Sign up [here](https://www.wrld3d.com/register/) for a free account and create an API key for your example apps. The API key is a string consisting of 32 alphanumeric characters. You will need to cut and paste the key into a resource file in order to authenticate your app. This is described in the ['Set your WRLD API key'](#_setApiKey1) step below.
* In Android Studio, select "Open..." and then select the top level android-api-samples folder.  If Android Studio is missing supporting libraries or components, you may be prompted to install these. Otherwise, Android Studio will download prerequisites automatically from JCenter.

You should now see two modules in the project: [helloworld](https://github.com/wrld3d/android-api-samples/tree/master/helloworld) and [apisamples](https://github.com/wrld3d/android-api-samples/tree/master/apisamples).

### HelloWorld
The [helloworld](https://github.com/wrld3d/android-api-samples/tree/master/helloworld) example is a basic app displaying an WRLD map. It demonstates how to integrate WRLD maps into your existing Android application.

#### <a name="_setApiKey1"></a>Set your WRLD API key
Edit the [```strings.xml```](https://github.com/wrld3d/android-api-samples/blob/master/helloworld/src/main/res/values/strings.xml#L4) file in the helloworld module and paste in your 32 character API key as the value for the ```eegeo_api_key``` resource.

#### Build and run
To build it, select "helloworld" in the "Run/Debug configuration" toolbar and click "Make Project". If you have a debuggable Android device attached, or if you are running an emulator, you can debug or run the app with the standard Android Studio tools.

For a step-by-step instructions which show how to create a basic app from scratch, see [our walkthrough documentation](https://docs.wrld3d.com/android/latest/docs/api/Walkthrough/).

### ApiSamples
The [apisamples](https://github.com/wrld3d/android-api-samples/tree/master/apisamples) app contains a collection of Activities, each illustrating an individual API feature.

#### Set your WRLD API key
Edit the [```strings.xml```](https://github.com/wrld3d/android-api-samples/blob/master/apisamples/src/main/res/values/strings.xml#L4) file in the apisamples module and paste in your 32 character API key as the value for the ```eegeo_api_key``` resource.

#### Build and run
To build the examples, ensure "apisamples" is selected in the "Run/Debug configuration" toolbar, then "Run->Run 'apisamples'".

## Further information
See our [API docs](https://docs.wrld3d.com/android/latest/docs/api/) for detailed class documentation and other information.

Questions, comments, or problems? All feedback is welcome -- just [create an issue](https://github.com/wrld3d/android-api-samples/issues).

## WRLD Android SDK package
These samples make use of the WRLD Android SDK, available as a Maven package via [Bintray](https://bintray.com/wrld/maven/wrld-android-sdk). 

[ ![Download](https://api.bintray.com/packages/wrld/maven/wrld-android-sdk/images/download.svg) ](https://bintray.com/wrld/maven/wrld-android-sdk/_latestVersion)

The gradle scripts included in this samples repo mean that the package is downloaded automatically by Android Studio, via JCenter.

The source for the SDK is available at https://github.com/wrld3d/android-api

## License
These examples are released under the Simplified BSD License. See the [LICENSE.md](https://github.com/wrld3d/android-api-samples/blob/master/LICENSE.md) file for details.
