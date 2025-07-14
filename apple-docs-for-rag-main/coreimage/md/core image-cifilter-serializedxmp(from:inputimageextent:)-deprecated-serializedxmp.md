

- Core Image
- CIFilter
-  serializedXMP(from:inputImageExtent:) Deprecated

Type Method

# serializedXMP(from:inputImageExtent:)

Serializes filter parameters into XMP form that is suitable for embedding in an image.

iOS 6.0–17.0DeprecatediPadOS 6.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.9–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func serializedXMP(
    from filters: [CIFilter],
    inputImageExtent extent: CGRect
) -> Data?
```

## Parameters 

`filters`  

The array of filters to serialize. See Discussion for the filters that can be serialized.

`extent`  

The extent of the input image to the filter.

## Discussion

At this time the only filters classes that can be serialized using this method are, CIAffineTransform, CICrop, and the filters returned by the CIImage methods `autoAdjustmentFilters()` and `autoAdjustmentFilters(options:)`. The parameters of other filter classes will not be serialized.

## See Also

### Deprecated

init!(cvPixelBuffer: CVPixelBuffer!, properties: [AnyHashable : Any]!, options: [CIRAWFilterOption : Any]!)

Creates a filter from a Core Video pixel buffer.

Deprecated

init!(imageData: Data!, options: [CIRAWFilterOption : Any]!)

Creates a filter that allows the processing of RAW images.

Deprecated

init!(imageURL: URL!, options: [CIRAWFilterOption : Any]!)

Creates a filter that allows the processing of RAW images.

Deprecated

struct CIRAWFilterOptionDeprecated

class func filterArray(fromSerializedXMP: Data, inputImageExtent: CGRect, error: NSErrorPointer) -> [CIFilter]

Returns an array of filter objects de-serialized from XMP data.

Deprecated

class func supportedRawCameraModels() -> [String]!Deprecated

