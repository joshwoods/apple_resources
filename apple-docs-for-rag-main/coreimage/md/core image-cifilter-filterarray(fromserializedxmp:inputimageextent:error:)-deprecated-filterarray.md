

- Core Image
- CIFilter
-  filterArray(fromSerializedXMP:inputImageExtent:error:) Deprecated

Type Method

# filterArray(fromSerializedXMP:inputImageExtent:error:)

Returns an array of filter objects de-serialized from XMP data.

iOS 6.0–17.0DeprecatediPadOS 6.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.9–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func filterArray(
    fromSerializedXMP xmpData: Data,
    inputImageExtent extent: CGRect,
    error outError: NSErrorPointer
) -> [CIFilter]
```

## Parameters 

`xmpData`  

The XMP data created previously by calling serializedXMP(from:inputImageExtent:).

`extent`  

The extent of the image from which the XMP data was extracted.

`outError`  

The address of an `NSError` object for receiving errors, otherwise `nil`.

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

class func supportedRawCameraModels() -> [String]!Deprecated

