

- Bundle Resources
- Information Property List
-  NSHandsTrackingUsageDescription 

Property List Key

# NSHandsTrackingUsageDescription

A message that tells the user why the app is requesting access to track the user’s hand position and location.

visionOS 1.0+

## Details 

Type  

string

## Discussion

Use this key to indicate that your app requires access to hand-tracking data. This includes hand skeleton, wrist, and forearm position and location. The first time your app tries to access hand-tracking data, the system prompts for permission. Provide a string for the prompt that explains why your app needs access. For more information on setting up ARKit for hand tracking, see Setting up access to ARKit data.

## See Also

### Vision

NSWorldSensingUsageDescription

A message that tells the user why the app is requesting access to image tracking, plane detection, or scene reconstruction.

