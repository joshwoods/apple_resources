

- AVFoundation
- AVMutableMovie
-  hasProtectedContent 

Instance Property

# hasProtectedContent

A Boolean value that indicates whether the asset contains protected content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
var hasProtectedContent: Bool { get }
```

## Discussion

Assets that contain protected content may not be playable without successful authorization, even if the value of its isPlayable property is true.

