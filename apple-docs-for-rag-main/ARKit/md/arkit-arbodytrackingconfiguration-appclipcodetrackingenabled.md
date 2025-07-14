

- ARKit
- ARBodyTrackingConfiguration
-  appClipCodeTrackingEnabled 

Instance Property

# appClipCodeTrackingEnabled

A Boolean value that indicates if the framework searches the physical environment for App Clip Codes.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
var appClipCodeTrackingEnabled: Bool { get set }
```

## Discussion

When this property’s value is true, the session delegate recieves an ARAppClipCodeAnchor via session(_:didAdd:) for every App Clip Code that ARKit detects in the physical environment. The default value is `false`.

Before calling this function, check that the configuration supports App Clip Code tracking by calling supportsAppClipCodeTracking.

To avoid scanning a physical code that’s not connected to an App Clip, the system ensures that an app provides an App Clip before allowing the app to interact with App Clip Codes. Without providing an App Clip, the app can recognize codes in the environment by determining their physical location (transform), but code URLs (url) remain `nil`.

## See Also

### Accessing App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

class var supportsAppClipCodeTracking: Bool

A flag that indicates if the device tracks App Clip Codes.

class ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

