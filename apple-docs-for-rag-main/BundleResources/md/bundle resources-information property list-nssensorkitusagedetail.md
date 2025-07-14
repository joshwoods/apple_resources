

- Bundle Resources
- Information Property List
-  NSSensorKitUsageDetail 

Property List Key

# NSSensorKitUsageDetail

A dictionary that includes keys for the specific information your app collects.

iOS 14.0+iPadOS 14.0+

## Details 

Type  

object

## Discussion

When your app attempts to read sensor information for the first time on a user’s device, the system presents a sheet that describes the information your app collects. You specify which information by defining an `Info.plist` key in this dictionary for each sensor your app uses, such as SRSensorUsageAmbientLightSensor. Users approve or deny your app’s ability to read private sensor information based on the description you provide for these properties.

For more information, see Configuring your project for sensor reading.

## Topics

### Device Activity

SRSensorUsageDeviceUsage

A collection of properties that explain your app’s need to observe how frequently a user’s device activates.

SRSensorUsageKeyboardMetrics

A collection of properties that explain your app’s need to observe the user’s keyboard activity.

SRSensorUsageWristDetection

A collection of properties that explain your app’s need to observe how the user wears their watch.

### App Activity

SRSensorUsageMessageUsage

A collection of properties that explain your app’s need to observe the user’s activity in Messages.

SRSensorUsagePhoneUsage

A collection of properties that explain your app’s need to observe the user’s phone activity.

### User Activity

SRSensorUsageECG

A collection of properties that explains your app’s need to observe the person’s electrocardiogram sensor data.

SRSensorUsageElevation

A collection of properties that explains your app’s need to observe the device’s elevation data.

SRSensorUsageFacialMetrics

A collection of properties that explains your app’s need to observe the user’s facial expressions.

SRSensorUsageHeartRate

A collection of properties that explains your app’s need to observe the user’s heart rate.

SRSensorUsageMediaEvents

A collection of properties that explains your app’s need to observe the user’s interactions with media, such as images and videos, in messaging apps.

SRSensorUsageMotion

A collection of properties that explain your app’s need to observe motion data.

SRSensorUsageOdometer

A collection of properties that explains your app’s need to observe the user’s odometer data.

SRSensorUsagePedometer

A collection of properties that explain your app’s need to observe steps information.

SRSensorUsagePPG

A collection of properties that explains your app’s need to observe the person’s photoplethysmogram sensor data.

SRSensorUsageSpeechMetrics

A collection of properties that explain your app’s need to analyze the user’s speech.

SRSensorUsageVisits

A collection of properties that explain your app’s need to observe the locations that the user frequents.

SRSensorUsageWristTemperature

A collection of properties that explains your app’s need to observe the user’s wrist temperature while the user sleeps.

### Environment

SRSensorUsageAmbientLightSensor

A collection of properties that explain your app’s need to observe light levels in the user’s environment.

## See Also

### Sensors

NSSensorKitUsageDescription

A short description of the purpose of your app’s research study.

NSSensorKitPrivacyPolicyURL

A hyperlink to a webpage that displays the privacy policy for your app’s research study.

