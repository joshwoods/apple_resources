

- AVFoundation
- AVCaptureOutput
-  outputRectConverted(fromMetadataOutputRect:) 

Instance Method

# outputRectConverted(fromMetadataOutputRect:)

Converts a rectangle in the coordinate system used for metadata outputs to one in the capture output object’s coordinate system.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func outputRectConverted(fromMetadataOutputRect rectInMetadataOutputCoordinates: CGRect) -> CGRect
```

## Parameters 

`rectInMetadataOutputCoordinates`  

A rectangle in the AVCaptureMetadataOutput coordinate system.

## Return Value

A rectangle in the AVCaptureOutput object’s coordinate system.

## Discussion

The rectangle of interest for an AVCaptureMetadataOutput object is in a coordinate system extending from `{0,0}` in the top-left to `{1,1}` in the bottom-right, relative to the device’s natural orientation. A capture output object uses a pixel coordinate space which you may zoom, rotate, or mirror.

## See Also

### Converting Between Coordinate Systems

func transformedMetadataObject(for: AVMetadataObject, connection: AVCaptureConnection) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

func metadataOutputRectConverted(fromOutputRect: CGRect) -> CGRect

Converts a rectangle in the capture output object’s coordinate system to one in the coordinate system used for metadata outputs.

