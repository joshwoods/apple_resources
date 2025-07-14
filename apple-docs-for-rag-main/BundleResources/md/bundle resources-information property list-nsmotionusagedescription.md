

- Bundle Resources
- Information Property List
-  NSMotionUsageDescription 

Property List Key

# NSMotionUsageDescription

A message that tells the user why the app is requesting access to the device’s motion data.

iOS 7.0+iPadOS 7.0+macOS 10.15+visionOS 1.0+

## Details 

Name  
Privacy - Motion Usage Description

Type  

string

## Discussion

Important

This key is required if your app uses APIs that access the device’s motion data, including CMSensorRecorder, CMPedometer, CMMotionActivityManager, and CMMovementDisorderManager. If you don’t include this key, your app will crash when it attempts to access motion data.

## See Also

### Motion

NSFallDetectionUsageDescription

A message to the user that explains the app’s request for permission to access fall detection event data.

**Name:** Fall Detection Usage Description

