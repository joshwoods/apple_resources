

- AVFoundation
-  AVVideoApertureMode 

Structure

# AVVideoApertureMode

A value that describes how a video is scaled or cropped.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVVideoApertureMode
```

## Topics

### Aperture Modes

static let cleanAperture: AVVideoApertureMode

The pixel aspect ratio and clean aperture will be applied.

static let encodedPixels: AVVideoApertureMode

The encoded dimensions of the image description are displayed.

static let productionAperture: AVVideoApertureMode

The pixel aspect ratio will be applied.

### Initializers

init(rawValue: String)

Creates a video aperture mode with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Presentation

var presentationSize: CGSize

The size at which the visual portion of the item is presented by the player.

var preferredMaximumResolution: CGSize

The desired maximum resolution of a video that is to be downloaded.

var videoApertureMode: AVVideoApertureMode

The video aperture mode to apply during playback.

