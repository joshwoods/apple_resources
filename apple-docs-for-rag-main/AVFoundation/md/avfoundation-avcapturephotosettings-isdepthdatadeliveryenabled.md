

- AVFoundation
- AVCapturePhotoSettings
-  isDepthDataDeliveryEnabled 

Instance Property

# isDepthDataDeliveryEnabled

A Boolean value that determines whether the photo output captures depth data along with the photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isDepthDataDeliveryEnabled: Bool { get set }
```

## Discussion

When this property is false (the default), the capture output produces only photo data and metadata.

If you change this property to true, the capture output records per-pixel scene depth information and delivers an AVDepthData object in the photo capture results. Enabling depth capture for a photo capture request requires that the photo output first be configured for depth capture using its own isDepthDataDeliveryEnabled property (and raises an exception otherwise).

Note

Enabling depth capture along with photo capture adds significant processing time before delivery of results to your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method.

## See Also

### Capturing Depth Data

var embedsDepthDataInPhoto: Bool

A Boolean value that determines whether any depth data captured with the photo is included when generating output file data.

var isDepthDataFiltered: Bool

A Boolean value that determines whether to smooth noise and fill in missing values in depth data output.

