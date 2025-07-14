

- AVFoundation
- AVCapturePhotoSettings
-  isDepthDataFiltered 

Instance Property

# isDepthDataFiltered

A Boolean value that determines whether to smooth noise and fill in missing values in depth data output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isDepthDataFiltered: Bool { get set }
```

## Discussion

When this property is true (the default), and depth data capture is enabled with the isDepthDataDeliveryEnabled property, the capture system smooths noise and fills in missing values (caused by low light or lens occlusion) in depth data maps by temporally interpolating between previous and subsequent frames of captured depth data.

Filtering depth data makes it more useful for applying visual effects to a companion image, but alters the data such that it may no longer be suitable for computer vision tasks. (In an unfiltered depth map, missing values are represented as `NaN`.) Set this property to false to disable filtering and receive unfiltered depth data.

## See Also

### Capturing Depth Data

var isDepthDataDeliveryEnabled: Bool

A Boolean value that determines whether the photo output captures depth data along with the photo.

var embedsDepthDataInPhoto: Bool

A Boolean value that determines whether any depth data captured with the photo is included when generating output file data.

