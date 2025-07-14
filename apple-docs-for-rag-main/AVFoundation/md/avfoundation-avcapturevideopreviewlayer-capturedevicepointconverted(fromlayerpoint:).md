

- AVFoundation
- AVCaptureVideoPreviewLayer
-  captureDevicePointConverted(fromLayerPoint:) 

Instance Method

# captureDevicePointConverted(fromLayerPoint:)

Converts a point from layer coordinates to the coordinate space of the capture device.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func captureDevicePointConverted(fromLayerPoint pointInLayer: CGPoint) -> CGPoint
```

## Parameters 

`pointInLayer`  

A point in layer coordinates to convert.

## Return Value

A point in capture device coordinates.

## Discussion

A capture device’s focusPointOfInterest and exposurePointOfInterest properties provide a CGPoint value where `{0,0}` represents the top-left and `{1,1}` represents the bottom-right of the unrotated image.

The conversion performed by this method takes the layer’s frame size and its videoGravity into consideration.

## See Also

### Converting Between Coordinate Spaces

func layerPointConverted(fromCaptureDevicePoint: CGPoint) -> CGPoint

Converts a point from the coordinate space of the capture device to the coordinate space of the layer.

func layerRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle from metadata output coordinates to the coordinate space of the layer.

func metadataOutputRectConverted(fromLayerRect: CGRect) -> CGRect

Converts a rectangle from layer coordinates to the coordinate space of the metadata output.

func transformedMetadataObject(for: AVMetadataObject) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

