

- Bundle Resources
- Information Property List
-  NSWorldSensingUsageDescription 

Property List Key

# NSWorldSensingUsageDescription

A message that tells the user why the app is requesting access to image tracking, plane detection, or scene reconstruction.

visionOS 1.0+

## Details 

Type  

string

## Discussion

Use this key to indicate that your app requires access to world-sensing data. This includes plane detection, image tracking, and scene-reconstruction anchors. The first time your app tries to access world-sensing data, the system prompts for permission. Provide a string for the prompt that explains why your app needs access. For more information on setting up ARKit for world sensing, see Setting up access to ARKit data.

Note

World tracking — unlike world sensing — doesn’t require authorization. For more information, see Tracking specific points in world space.

## See Also

### Vision

NSHandsTrackingUsageDescription

A message that tells the user why the app is requesting access to track the user’s hand position and location.

