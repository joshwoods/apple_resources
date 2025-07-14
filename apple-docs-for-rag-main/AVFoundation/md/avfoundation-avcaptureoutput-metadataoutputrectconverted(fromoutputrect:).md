

- AVFoundation
- AVCaptureOutput
-  metadataOutputRectConverted(fromOutputRect:) 

Instance Method

# metadataOutputRectConverted(fromOutputRect:)

Converts a rectangle in the capture output object’s coordinate system to one in the coordinate system used for metadata outputs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func metadataOutputRectConverted(fromOutputRect rectInOutputCoordinates: CGRect) -> CGRect
```

## Parameters 

`rectInOutputCoordinates`  

A rectangle in the AVCaptureOutput object’s coordinate system.

## Return Value

A rectangle in the AVCaptureMetadataOutput coordinate system.

## Discussion

An AVCaptureMetadataOutput object expresses its rectOfInterest as a CGRect where 0,0 represents the top-left of the picture area, and 1,1 represents the bottom-right on an unrotated picture. This convenience method converts a rectangle in the coordinate space of the output to a rectangle of interest in the coordinate space of a metadata output whose capture device provides input to the output. The conversion takes orientation, mirroring, and scaling into consideration.

See transformedMetadataObject(for:connection:) for a full discussion of how the system applies orientation and mirroring to sample buffers passing through the output.

## See Also

### Converting Between Coordinate Systems

func transformedMetadataObject(for: AVMetadataObject, connection: AVCaptureConnection) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

func outputRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle in the coordinate system used for metadata outputs to one in the capture output object’s coordinate system.

