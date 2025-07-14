

- Xcode
- Capabilities
-  Configuring background execution modes 

Article

# Configuring background execution modes

Indicate the background services your app requires to continue executing in the background in iOS, iPadOS, tvOS, visionOS, and watchOS.

## Overview

Typically, an app is in a suspended state when it’s in the background. However, there are a limited number of background execution modes your app can support that enable it to run when in the background, such as playing audio, receiving location updates, or processing scheduled tasks. For apps that adopt one or more of these modes, the system launches or resumes the app, in the background, and affords it time to process any related events.

Use background execution modes sparingly because overuse can negatively impact device performance and battery life. If an alternative to executing in the background exists, use the alternative instead. For example, apps can use the significant-change location service to receive location events as an alternative to using the Location updates background mode.

Before you can select the background execution modes your app requires, follow the steps in Add a capability to add the Background Modes capability to your app’s target.

The background execution modes that appear after you add the capability depend on the target’s platform. For watchOS apps with separate WatchKit extensions, you need to add the capability to the WatchKit Extension target.

Note

The Background Modes capability isn’t available for macOS apps.

### Specify the background modes your app requires

Before your app can leverage one or more background execution modes, you need to declare the modes it requires by performing the following:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Background Modes capability.

5.  Select one or more background execution modes using the corresponding checkboxes.

6.  For watchOS apps, choose the appropriate session type from the pop-up menu. For more information, see Using extended runtime sessions.

Xcode adds the UIBackgroundModes array to your app’s `Info.plist` file, if it isn’t already present, and uses the modes you select to populate the array with the necessary values.

Apple’s platforms support these background execution modes:

| Mode | Value | Description | Platforms |
|----|----|----|----|
| Audio, AirPlay, and Picture in Picture | `audio` | The app plays audible content in the background. For more information, see Configuring your app for media playback. | iOS, iPadOS, tvOS, visionOS |
| Audio | `audio` | The app plays audible content in the background. For more information, see Playing Background Audio. | watchOS |
| Location updates | `location` | The app provides location-based information and requires the use of the platform’s standard location service. For more information, see Configuring your app to use location services. | iOS, iPadOS, watchOS |
| Voice over IP | `voip` | The app provides Voice over IP services. For more information, see the CallKit framework. | iOS, iPadOS, visionOS, watchOS |
| External accessory communication | `external-accessory` | The app communicates with an accessory that delivers data at regular intervals. For more information, see the External Accessory framework. | iOS, iPadOS |
| Uses Bluetooth LE accessories | `bluetooth-central` | The app communicates with a Bluetooth accessory while in the background. For more information, see the Core Bluetooth framework. | iOS, iPadOS, visionOS |
| Acts as a Bluetooth LE accessory | `bluetooth-peripheral` | The app uses peripheral mode to communicate with a Bluetooth accessory. For more information, see the Core Bluetooth framework. | iOS, iPadOS |
| Background fetch | `fetch` | The app requires new content from the network at regular intervals. For more information, see Using background tasks to update your app. | iOS, iPadOS, tvOS, visionOS |
| Remote notifications | `remote-notification` | The app uses push notifications as a signal that new content is available to download. For more information, see Pushing background updates to your App. | iOS, iPadOS, tvOS, visionOS, watchOS |
| Background processing | `processing` | The app executes scheduled tasks while in the background. For more information, see BGTaskScheduler. | iOS, iPadOS, tvOS, visionOS |
| Workout processing | `workout-processing` | The app uses a workout session to track a user’s activity on Apple Watch. For more information, see Running workout sessions. | watchOS |
| Uses Nearby Interaction | `nearby-interaction` | The app locates and interacts with nearby devices. For more information, see the Nearby Interaction framework. | iOS, iPadOS |
| Push to Talk | `push-to-talk` | The app launches in response to a push notification and plays audible content in the background. For more information, see the Push to Talk framework. | iOS, iPadOS |

## See Also

### App execution

Configuring custom fonts

Register your app as a provider or consumer of systemwide custom fonts.

Configuring game controllers

Enhance gameplay input by enabling the discovery, configuration, and use of physical game controllers.

Configuring Maps support

Register your iOS routing app to provide point-to-point directions to Maps and other apps.

Configuring Siri support

Enable your app and its Intents extension to resolve, confirm, and handle user-driven Siri requests for your app’s services.

