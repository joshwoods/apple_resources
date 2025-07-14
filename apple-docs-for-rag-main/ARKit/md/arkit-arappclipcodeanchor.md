

- ARKit
-  ARAppClipCodeAnchor 

Class

# ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
class ARAppClipCodeAnchor
```

## Overview

Your App Clip gives users immediate access to critical or context-specific parts of your app’s AR experience, and makes it easy for them to download and launch your full app if they choose.

You can use physical App Clip Codes in the real world to enable users to discover your App Clip. An App Clip Code includes a unique URL and can incorporate an NFC tag. When users hold their iPhone near the code or scan it with the camera or Code Scanner in Control Center, the system offers to launch the code’s associated App Clip.

For more on App Clip Codes, see App Clips. For an app that reacts to App Clip Codes in AR, see Interacting with App Clip Codes in AR.

### Distinguish Between App Clip Codes

There may be multiple App Clip Codes visible in the camera feed that share the same url, so ARKit also relies on the App Clip Code’s location (see transform) to distinguish different App Clip Codes in the physical environment.

When the framework recognizes an App Clip Code, it initializes an ARAppClipCodeAnchor and passes it to the session delegate via session(_:didAdd:). If a recognized App Clip Code becomes obscured or is no longer visible in the camera feed, the framework sets the anchor’s isTracked property to false and passes it into the session(_:didUpdate:) callback. If the same App Clip Code becomes visible once again:

- ARKit sets isTracked to true if the App Clip Code maintained its relative position in the physical environment.

- ARKit intializes a new ARAppClipCodeAnchor if the App Clip Code position in the physical environment changed significantly.

### Remove App Clip Codes

To prevent App Clip Codes from accumulating in the session, ARKit removes anchors by passing them in to the session(_:didRemove:) callback. ARKit removes an ARAppClipCodeAnchor if all of the following conditions are true:

- The framework instantiates a new ARAppClipCodeAnchor.

- The new anchor’s url matches one or more existing anchors with substantially different positions in the physical environment.

- The existing anchors are untracked (isTracked is false).

## Topics

### Decoding the URL

var url: URL?

The URL encoded in an App Clip Code.

var urlDecodingState: ARAppClipCodeAnchor.URLDecodingState

A state that indicates the process of decoding an App Clip Code URL.

enum URLDecodingState

The states in the process of decoding an App Clip code URL.

### Measuring Physical Size

var radius: Float

The App Clip Code’s radius in meters.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- ARTrackable
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

