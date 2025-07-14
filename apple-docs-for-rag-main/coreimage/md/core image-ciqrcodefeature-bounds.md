

- Core Image
- CIQRCodeFeature
-  bounds 

Instance Property

# bounds

A rectangle indicating the position and extent of the feature in image coordinates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var bounds: CGRect { get }
```

## Discussion

This property identifies the rectangular region *of the image* containing the detected barcode, not necessarily the shape of the barcode. A detected barcode is rectangular in space, but may appear in perspective in the image. Use the properties listed in Identifying the Corners of a Detected Barcode to find the corners of the barcode as it appears in perspective.

