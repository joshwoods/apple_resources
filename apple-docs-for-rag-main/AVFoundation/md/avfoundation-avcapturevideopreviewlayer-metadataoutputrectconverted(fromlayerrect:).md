

- AVFoundation
- AVCaptureVideoPreviewLayer
-  metadataOutputRectConverted(fromLayerRect:) 

Instance Method

# metadataOutputRectConverted(fromLayerRect:)

Converts a rectangle from layer coordinates to the coordinate space of the metadata output.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func metadataOutputRectConverted(fromLayerRect rectInLayerCoordinates: CGRect) -> CGRect
```

## Parameters 

`rectInLayerCoordinates`  

A rectangle in the AVCaptureVideoPreviewLayer object’s coordinate system.

## Return Value

A rectangle in the metadata output’s coordinate system.

## Discussion

A metadata capture output’s rectOfInterest a CGRect value where `{0,0}` represents the top-left of the picture area, and `{1,1}` represents the bottom-right on an unrotated image.

The system takes the layer’s frame size and its videoGravity into consideration when making the conversion.

## See Also

### Converting Between Coordinate Spaces

func layerPointConverted(fromCaptureDevicePoint: CGPoint) -> CGPoint

Converts a point from the coordinate space of the capture device to the coordinate space of the layer.

func captureDevicePointConverted(fromLayerPoint: CGPoint) -> CGPoint

Converts a point from layer coordinates to the coordinate space of the capture device.

func layerRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle from metadata output coordinates to the coordinate space of the layer.

func transformedMetadataObject(for: AVMetadataObject) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

