

- MusicKit
- MusicLibrary
- MusicLibrary.Error
-  MusicLibrary.Error.permissionDenied 

Case

# MusicLibrary.Error.permissionDenied

An error that occurs when the user doesn’t consent for the current app to access their Apple Music library.

iOS 16.1+iPadOS 16.1+Mac Catalyst 17.0+macOS 14.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
case permissionDenied
```

## Discussion

Apps using MusicKit need to request prior informed consent from the user to access their Apple Music library by calling request() at the appropriate point in the app flow, right before needing to use other APIs from MusicKit.

