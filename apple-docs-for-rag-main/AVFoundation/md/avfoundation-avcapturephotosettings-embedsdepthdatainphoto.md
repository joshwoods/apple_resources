

- AVFoundation
- AVCapturePhotoSettings
-  embedsDepthDataInPhoto 

Instance Property

# embedsDepthDataInPhoto

A Boolean value that determines whether any depth data captured with the photo is included when generating output file data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var embedsDepthDataInPhoto: Bool { get set }
```

## Mentioned in 

Capturing Photos with Depth

## Discussion

When this property is true (the default), and depth data capture is enabled with the isDepthDataDeliveryEnabled property, the AVCapturePhoto class includes the depth map as an embedded attachment when you flatten the photo data for output in compatible file formats.

Set this property to false if you wish to capture depth data with a photo but not include depth data in output.

## See Also

### Capturing Depth Data

var isDepthDataDeliveryEnabled: Bool

A Boolean value that determines whether the photo output captures depth data along with the photo.

var isDepthDataFiltered: Bool

A Boolean value that determines whether to smooth noise and fill in missing values in depth data output.

