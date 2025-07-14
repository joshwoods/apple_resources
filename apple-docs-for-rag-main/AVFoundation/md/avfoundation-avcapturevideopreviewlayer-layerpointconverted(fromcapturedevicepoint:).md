

- AVFoundation
- AVCaptureVideoPreviewLayer
-  layerPointConverted(fromCaptureDevicePoint:) 

Instance Method

# layerPointConverted(fromCaptureDevicePoint:)

Converts a point from the coordinate space of the capture device to the coordinate space of the layer.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func layerPointConverted(fromCaptureDevicePoint captureDevicePointOfInterest: CGPoint) -> CGPoint
```

## Parameters 

`captureDevicePointOfInterest`  

A point in capture device coordinates to convert.

## Return Value

A point in layer coordinates.

## Discussion

A capture device’s focusPointOfInterest and exposurePointOfInterest properties provide a CGPoint value where `{0,0}` represents the top-left and `{1,1}` represents the bottom-right of the unrotated image.

The system takes the layer’s frame size and its videoGravity into consideration when making the conversion.

## See Also

### Converting Between Coordinate Spaces

func captureDevicePointConverted(fromLayerPoint: CGPoint) -> CGPoint

Converts a point from layer coordinates to the coordinate space of the capture device.

func layerRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle from metadata output coordinates to the coordinate space of the layer.

func metadataOutputRectConverted(fromLayerRect: CGRect) -> CGRect

Converts a rectangle from layer coordinates to the coordinate space of the metadata output.

func transformedMetadataObject(for: AVMetadataObject) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

