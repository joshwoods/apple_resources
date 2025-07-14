

- AVFoundation
-  AVLayerVideoGravity 

Structure

# AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVLayerVideoGravity
```

## Topics

### Video Gravities

static let resize: AVLayerVideoGravity

The video stretches to fill the layer’s bounds.

static let resizeAspect: AVLayerVideoGravity

The video preserves its aspect ratio and fits it within the layer’s bounds.

static let resizeAspectFill: AVLayerVideoGravity

The video preserves its aspect ratio and fills the layer’s bounds.

### Initializers

init(rawValue: String)

Creates a video gravity with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the Presentation

var videoRect: CGRect

The current size and position of the video image that displays within the layer’s bounds.

var videoGravity: AVLayerVideoGravity

A value that specifies how the layer displays the player’s visual content within the layer’s bounds.

