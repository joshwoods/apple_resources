

- MusicKit
- MusicAuthorization
- MusicAuthorization.Status
-  MusicAuthorization.Status.denied 

Case

# MusicAuthorization.Status.denied

The user denied permission for the current app to use MusicKit.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case denied
```

## Discussion

On iOS, applications may attempt to recover from this situation by suggesting to their users that they can grant access to their Apple Music data again by linking to openSettingsURLString.

