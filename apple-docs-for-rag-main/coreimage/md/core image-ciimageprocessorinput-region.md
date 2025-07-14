

- Core Image
- CIImageProcessorInput
-  region 

Instance Property

# region

The area within the input image to be processed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var region: CGRect { get }
```

**Required**

## Discussion

This region will always contain, but may be larger than, the region produced by the `roiCallback` block parameter of the `withExtent(_:processorDescription:argumentDigest:inputFormat:outputFormat:options:roiCallback:processor:)` method.

## See Also

### Getting Supplemental Information for Image Processing

var bytesPerRow: Int

The number of bytes per row of pixels in the input image data.

**Required**

var format: CIFormat

The per-pixel data format of the image to be processed.

**Required**

