

- AVFoundation
- AVPlayerItemOutput
-  suppressesPlayerRendering 

Instance Property

# suppressesPlayerRendering

A Boolean value that indicates whether the player object renders the receiver’s output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var suppressesPlayerRendering: Bool { get set }
```

## Discussion

When the value of this property is false (the default), the player object handles the rendering of the receiver’s associated output. Change the value of this property to true to suppress the rendering of the media data associated with this object.

