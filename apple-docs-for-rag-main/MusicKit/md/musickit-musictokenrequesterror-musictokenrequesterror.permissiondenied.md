

- MusicKit
- MusicTokenRequestError
-  MusicTokenRequestError.permissionDenied 

Case

# MusicTokenRequestError.permissionDenied

An error that occurs when the user doesn’t consent for the current app to access their Apple Music data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case permissionDenied
```

## Discussion

Apps using MusicKit need to request prior informed consent from the user to access their Apple Music data by calling request() at the appropriate point in the app flow, right before needing to use other APIs from MusicKit.

