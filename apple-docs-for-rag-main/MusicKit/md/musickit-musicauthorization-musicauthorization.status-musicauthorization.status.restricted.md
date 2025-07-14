

- MusicKit
- MusicAuthorization
- MusicAuthorization.Status
-  MusicAuthorization.Status.restricted 

Case

# MusicAuthorization.Status.restricted

Apps on this device can’t access MusicKit in a way that the user can’t change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case restricted
```

## Discussion

In this scenario, don’t prompt for authorization.

An example of this situation is when the device is in education mode.

