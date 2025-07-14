

- SensorKit
-  Configuring your project for sensor reading 

Article

# Configuring your project for sensor reading

Add metadata to your app to attain system and user permission to access sensor data.

## Overview

If Apple approves your idea for a research-study app, you can read sensor data from devices after receiving the userʼs permission. Once Apple approves your app, you receive an entitlement that enables your app to read sensor data. In accordance with the approval, you also need to comply with Appleʼs privacy policy.

When your app attempts to read sensor information for the first time on a person’s device, the system presents a sheet that explains your app’s research study and the information your app collects. The sheet prompts people to approve access to personal information at a granular level, and your app needs to tell people which information is essential to the study. You supply the study purpose, requested sensors, and privacy policy URL in the project’s `Info.plist`.

For more information, see Sensor &amp; Usage Data &amp; Privacy.

### Request the sensor reader entitlement

To use SensorKit, the OS requires the com.apple.developer.sensorkit.reader.allow entitlement in your app’s code signature. Apple only grants the entitlement for approved research studies. If you’re interested in accessing SensorKit data for your study, submit a research proposal and request the entitlement. For more information, see Accessing SensorKit Data.

### Create a manual provisioning profile

Xcode requires a manual provisioning profile that includes an explicit App ID to code-sign your app with the sensor reader entitlement.

To create the explicit App ID, sign in to Apple Developer, register an App ID for your SensorKit project, and enable the sensor reader entitlement under Additional Capabilities on the Certificates, Identifiers, &amp; Profiles page. For more information, see Register an App ID.

To create the manual provisioning profile, select Profiles from the sidebar, click the add button (+) in the upper-left, and select the iOS App Development profile type. For more information, see Create a development provisioning profile.

Install the provisioning profile by downloading it and dragging it on to the Xcode icon in the Dock. Alternatively, you can select the Download Manual Profiles option by choosing Xcode \> Preferences \> Accounts and selecting your Apple ID and applicable team. For more information, see Download manual provisioning profiles.

### Configure Xcode for signing

Define a bundle ID in Xcode for your App ID by selecting your target in the project editor and clicking General. For more information, see Set the bundle ID.

Add a new property list file to your project named `[Your App Name].entitlements` if it doesn’t already exist. Add a key titled `com.apple.developer.sensorkit.reader.allow` with the type Array, and add a string value for each sensor your app uses:

```
```

The code-signing entitlements file for the above raw property list appears as follows in Xcode:

To sign your app with the manual provisioning profile and sensor reader entitlement, set your targetʼs build settings as follows:

- Code Signing Entitlements to the entitlements file

- Code Signing Identity to `Apple Developer`

- Code Signing Style to `Manual`

- Provisioning Profile to the manual provisioning profile you created

### Describe the purpose of your study

The system presents the Research Sensor & Usage Data Request sheet that introduces your appʼs study to people. Define a short description of your appʼs research purpose with the usage description `Info.plist` key.

```
```

The sheet displays the research purpose in the App Research Purpose banner.

### Link your app’s privacy policy

Add a link to your privacy-policy webpage in your projectʼs `Info.plist` using the NSSensorKitPrivacyPolicyURL key.

```
```

The sheet displays a link to your app’s privacy policy below the description of your study.

### Explain how your app uses the data

The sheet also explains what your app intends to do with the information it collects with a particular sensor. You provide this intent per sensor by adding the sensorʼs usage-detail key in your appʼs `info.plist`. For example, add the SRSensorUsageMotion key when you use the accelerometer property. For the other sensor-specific usage keys, see the SRSensor property descriptions.

```
```

To begin reading sensor data, call `requestAuthorization(sensors:completion:)` to pass in the sensors your app records.

```
```

The first time your app requests authorization for a particular sensor, the sheet prompts for user approval and displays the sensorʼs corresponding usage-detail string.

### Specify the sensors your app requires

Through the sheet, people approve each sensor individually by tapping Allow Collection & Sharing or Don’t Allow Collection & Sharing.

By specifying whether your study requires one or more of the sensors, people can opt out, participate partially, or fully opt in. To indicate that your study requires a sensor, add a Boolean key titled `Required` to the sensorʼs usage-detail dictionary with a value of `true`.

```
```

For sensor information that’s optional to your study, you can omit the `Required` key or set its value to `false`.

If a person disapproves of a required sensor, the system warns them that the study requires the information. In the prompt, they have the option to not enroll or to reconsider by tapping Change Choice.

After a person answers the prompt, they can adjust authorization status per sensor later by choosing Settings \> Privacy \> Research Sensor & Usage Data.

## See Also

### Setup

class SRSensorReader

An object that establishes user authorization and records data for a particular sensor.

