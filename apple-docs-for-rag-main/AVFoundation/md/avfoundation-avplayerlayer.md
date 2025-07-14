

- AVFoundation
-  AVPlayerLayer 

Class

# AVPlayerLayer

An object that presents the visual contents of a player object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVPlayerLayer
```

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Overview

A common way to use this object in iOS or tvOS is as the backing layer for a UIView, as the following example shows:

```
/// A view that displays the visual contents of a player object.
class PlayerView: UIView {

    // Override the property to make AVPlayerLayer the view's backing layer.
    override static var layerClass: AnyClass { AVPlayerLayer.self }

    // The associated player object.
    var player: AVPlayer? {
        get { playerLayer.player }
        set { playerLayer.player = newValue }
    }

    private var playerLayer: AVPlayerLayer { layer as! AVPlayerLayer }
}
```

Important

The value of a player layer’s inherited contents property is opaque and you can’t change it.

## Topics

### Creating a Player Layer

init(player: AVPlayer?)

Creates a layer object to present the visual contents of a player’s current item.

### Configuring the Presentation

var videoRect: CGRect

The current size and position of the video image that displays within the layer’s bounds.

var videoGravity: AVLayerVideoGravity

A value that specifies how the layer displays the player’s visual content within the layer’s bounds.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

### Determining Display Readiness

var isReadyForDisplay: Bool

A Boolean value that indicates whether the first video frame of the player’s current item is ready for display.

### Accessing the Player

var player: AVPlayer?

The player whose visual content the layer displays.

### Processing Pixel Buffers

var pixelBufferAttributes: [String : Any]?

The attributes of the visual output that displays in the player layer during playback.

func displayedPixelBuffer() -> CVPixelBuffer?

Returns the pixel buffer that the player layer currently displays.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Presentation

Monitoring playback progress in your app

Observe the playback of a media asset to update your app’s user-interface state.

Using HEVC Video with Alpha

Play, write, and export HEVC video with an alpha channel to add overlay effects to your video processing.

class AVSynchronizedLayer

A Core Animation layer that derives its timing from a player item so that you can synchronize layer animations with media playback.

