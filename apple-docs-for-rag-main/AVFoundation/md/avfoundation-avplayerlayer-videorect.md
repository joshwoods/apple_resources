

- AVFoundation
- AVPlayerLayer
-  videoRect 

Instance Property

# videoRect

The current size and position of the video image that displays within the layer’s bounds.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var videoRect: CGRect { get }
```

## Discussion

The size and position of a rectangle depends on the aspect ratio of the media (16:9 or 4:3), the layer’s bounds, and the value of its videoGravity property.

This property is key-value observable.

## See Also

### Configuring the Presentation

var videoGravity: AVLayerVideoGravity

A value that specifies how the layer displays the player’s visual content within the layer’s bounds.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

