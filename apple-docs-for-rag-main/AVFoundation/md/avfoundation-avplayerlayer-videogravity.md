

- AVFoundation
- AVPlayerLayer
-  videoGravity 

Instance Property

# videoGravity

A value that specifies how the layer displays the player’s visual content within the layer’s bounds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var videoGravity: AVLayerVideoGravity { get set }
```

## Discussion

A player layer supports the following video gravity values:

- resizeAspect

- resizeAspectFill

- resize

The default value is resizeAspect.

This property is animatable.

## See Also

### Configuring the Presentation

var videoRect: CGRect

The current size and position of the video image that displays within the layer’s bounds.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

