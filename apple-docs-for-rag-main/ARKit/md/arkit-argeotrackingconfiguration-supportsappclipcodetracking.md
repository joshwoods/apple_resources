

- ARKit
- ARGeoTrackingConfiguration
-  supportsAppClipCodeTracking 

Type Property

# supportsAppClipCodeTracking

A flag that indicates if the device tracks App Clip Codes.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
class var supportsAppClipCodeTracking: Bool { get }
```

## Discussion

Devices require the Apple Neural Engine (ANE) to track App Clip Codes. The system sets this property to true if the device contains the ANE chip. The default value of this property is false.

Call this function before setting appClipCodeTrackingEnabled.

## See Also

### Accessing App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

var appClipCodeTrackingEnabled: Bool

A Boolean value that indicates if the framework searches the physical environment for App Clip Codes.

class ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

