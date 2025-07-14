

- Core Motion
-  Accessing submersion data 

Article

# Accessing submersion data

Use a water-submersion manager to receive water pressure, temperature, and depth data on Apple Watch Ultra.

## Overview

Apple Watch Ultra can collect water pressure, depth, and temperature data while submerged; however, before your app can access this data, you need to perform the following setup steps:

- Include an Apple-supplied entitlement that grants access to the submersion data.

- Provide an information property list key that describes why the app needs access to submersion data.

- Add the `underwater-depth` Background Mode capability to the app.

- Verify that the submersion manager is available on the current device.

To start monitoring submersion data, instantiate a CMWaterSubmersionManager and assign a delegate to the submersion manager. The system begins sending updates to your delegate. You can then start an extended runtime session when the watch first submerges, and transition your app to a touchless user interface for the duration of the dive.

### Add the required entitlement

Before you can instantiate the CMWaterSubmersionManager class, your app needs to include a Submerged Depth and Pressure entitlement to access submersion data.

To access data for dives with a maximum depth of 6 meters, add the Shallow Depth and Pressure capability to your app. For more information, see Adding capabilities to your app.

To enable a maximum depth of 40 meters, you need to apply for the full Submersion Depth and Pressure entitlement. For more information, see the Submerged Depth and Pressure entitlement request form.

If you instantiate the manager without an entitlement, the system calls your delegate’s manager(_:errorOccurred:) method, passing a CMErrorNotEntitled error, and your delegate doesn’t receive any additional data.

### Authorize access to motion data

The system automatically asks the wearer for authorization to access motion data when you first instantiate a CMWaterSubmersionManager; however, before you can instantiate the manager, you need to include the NSMotionUsageDescription key in your app target’s information property list and provide a usage description string.

The system displays this usage description when it prompts the wearer for authorization to access motion data. If you don’t include a usage description string, your app crashes when you try to instantiate a CMWaterSubmersionManager object.

### Add support for the underwater depth extended runtime session

To make sure your app continues to run, and remains visible, you need to add the `underwater-depth` Background Mode to your app’s `Info.plist` file. This background mode lets your app run as the frontmost app during a dive session.

Open the `Info.plist` file as XML by Control-clicking it in the Project navigator and selecting Open As \> Source Code. Next, edit the string value for the WKBackgroundModes key so that it contains the `underwater-depth` value.

```
```

If your app doesn’t already have an `Info.plist` file, you can add a placeholder, and then edit it using the following steps:

1.  Select your app’s WatchKit Extension target and click the Signing & Capabilities tab.

2.  Choose Editor \> Add Capability and double-click the Background Modes capability to add it to the Signing & Capabilities pane.

3.  Choose an option to use as a placeholder from the Session Type pop-up menu. The `Info.plist` file appears in the Project navigator.

4.  Open the `Info.plist` file as XML source code and replace the placeholder string value for the WKBackgroundModes key with the `underwater-depth` value.

Adding the `underwater-depth` Background Mode capability to your `Info.plist` file lets your app run an extended runtime session so that it can remain the frontmost app for the duration of the dive session. It also adds your app to the list of apps that the system can autolaunch when the wearer submerges the watch.

Unlike most extended runtime sessions, your app doesn’t need to start an extended runtime session to gain additional time as the frontmost app. Just by adding this key, the system automatically keeps your app as the frontmost app for 30 minutes after the wearer launches it. This gives the wearer time to prepare for the dive before submerging. Then, after you start an extended runtime session, your app remains the frontmost app for the duration of the dive. The session doesn’t time out until the watch spends more than 10 minutes unsubmerged or the wearer turns off Water Lock.

If you don’t explicitly start an extended runtime session, the system automatically starts a runtime session when the wearer dives below 1 meter, and your app transitions to the CMWaterSubmersionMeasurement.DepthState.submergedDeep state.

### Verify that the submersion data is available on the current device.

Before creating a submersion manager, verify that the data is available on the current device.

```
```

On Apple Watch Ultra, the system sets waterSubmersionAvailable to true. On all other devices and in Simulator, the system sets it to false.

### Start monitoring submersion data

To begin receiving submersion data, instantiate a CMWaterSubmersionManager object and assign a CMWaterSubmersionManagerDelegate.

```
```

Your delegate begins to receive data as soon as you assign it. For example, your delegate receives both event notifications and errors.

```
```

Your delegate also begins receiving measurement updates. If the watch isn’t submerged, the updates only include surface pressure and submersion state data. After submersion, it also receives water pressure and depth data. The system sends measurement updates three times a second while the watch is submerged. When the watch is on the surface, the system provides updates at a slower rate, and may stop providing updates if the watch isn’t moving.

```
```

The watch also receives water temperature data when it’s submerged.

```
```

The water temperature readings can take some time to converge on the correct value. The system estimates how long it takes to converge to the correct results, and calculates an uncertainty value based on the expected convergence.

### Start a dive session

You can start an extended runtime session as the wearer begins their dive.

```
```

This session continues to run until:

- You explicitly cancel the session by calling invalidate() on it.

- The wearer turns off Water Lock.

- Your app remains in the CMWaterSubmersionEvent.State.notSubmerged state for at least 10 minutes.

For more information, see Using extended runtime sessions.

### Transition to a touchless user interface

Starting an extended runtime session automatically enables Water Lock on the watch. As a result, the system disables the watch’s touchscreen for the duration of the dive. If you want the wearer to interact with your app during the dive, you need to enable interaction using either the Digital Crown or the Action button.

Many views, like List, ScrollView, and Picker, automatically respond to the Digital Crown. The wearer can interact with these elements without needing any changes to the user interface.

```
```

You can also use the digitalCrownRotation(_:) view modifier to respond directly when the wearer rotates the Digital Crown.

```
```

For the Action button, implement a StartDiveIntent to launch your app and prepare for a new dive when the wearer first presses the Action button. You can then donate an AppIntent for the Action button’s next action. If the wearer presses the Action button any other time during the session, it triggers the next action. Your app can have only one next action at a time, and donating a new intent changes the next action — letting you customize the next action based on your app’s current state.

```
```

For more information, see Responding to the Action button on Apple Watch Ultra.

### Handle automatic dive sessions

If you don’t explicitly start an extended runtime session, the system automatically starts a session when the wearer descends below 1 meter. It then passes the session to your app delegate’s handle(_:) method. To use this session, add a delegate and save it to a variable that remains in scope for the entire dive’s duration.

```
```

### Respond to autolaunch

On Apple Watch Ultra, the wearer can tell the system to launch an app when the watch becomes submerged. To enable this feature, they choose Settings \> General \> Auto-Launch and select the Auto-Launch App setting from the When Submerged group. They can also select which app the system launches.

The system adds your app to the list of autolaunchable apps as soon as you add the `underwater-depth` Background Mode capability to your app’s `Info.plist` file. This means your app needs to respond appropriately if the wearer sets it as the autolaunch app, and jumps into the water without otherwise interacting with your app.

For example, you can set up your app’s CMWaterSubmersionManager when your app launches. This ensures that your app is always ready to receive submersion data. Then, when the wearer descends below 1 meter, you can use your handle(_:) method to grab the automatically generated extended runtime session. Alternatively, if you prefer to explicitly start your own extended runtime session, you can start the session when your app receives a CMWaterSubmersionEvent.State.submerged event.

### Test submersion data

Always test submersion data on Apple Watch Ultra. You can’t instantiate the submersion manager in Simulator. To trigger a submersion event, you need to submerge Apple Watch Ultra in a tank of water at least 1 foot deep. When testing in a pressurized container, make sure the watch is completely submerged in water.

If the water isn’t deep enough to trigger a submersion event, you can enable Easy Submersion mode using a paired iPhone. Connect the phone to your Mac and in Xcode 14.2 or later, select Debug \> Induce Device Conditions \> Easy Submersion \> Enable Easy Submersion.

## See Also

### Water submersion

class CMWaterSubmersionManager

An object for managing the collection of pressure and temperature data during submersion.

protocol CMWaterSubmersionManagerDelegate

A delegate that receives updates about ambient pressure, water pressure, water temperature, and submersion events.

class CMWaterSubmersionEvent

An event indicating that the device’s submersion state has changed.

class CMWaterSubmersionMeasurement

An update that contains data about the pressure and depth.

class CMWaterTemperature

An update that contains data about the water temperature.

