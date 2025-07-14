

- Core Image
- CIFilter
-  supportedRawCameraModels() Deprecated

Type Method

# supportedRawCameraModels()

iOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func supportedRawCameraModels() -> [String]!
```

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

class func serializedXMP(from: [CIFilter], inputImageExtent: CGRect) -> Data?

Serializes filter parameters into XMP form that is suitable for embedding in an image.

Deprecated

class func filterArray(fromSerializedXMP: Data, inputImageExtent: CGRect, error: NSErrorPointer) -> [CIFilter]

Returns an array of filter objects de-serialized from XMP data.

Deprecated

