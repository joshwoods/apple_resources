

- Core Image
- CIFilter
-  init(imageData:options:) Deprecated

Initializer

# init(imageData:options:)

Creates a filter that allows the processing of RAW images.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init!(
    imageData data: Data!,
    options: [CIRAWFilterOption : Any]! = [:]
)
```

Deprecated

Use init(imageData:identifierHint:) instead.

## Parameters 

`data`  

The RAW image data to initialize the object with.

`options`  

An options dictionary.

## Return Value

A `CIFilter` object.

## Discussion

You can pass any of the keys defined in RAW Image Options along with the appropriate value in `options`. You should provide a source type identifier hint key (`kCGImageSourceTypeIdentifierHint`) and the appropriate source type value to help the decoder determine the file type. Otherwise it’s possible to obtain incorrect results.

The first step when working with RAW images in Core Image is to process the image using either init(imageData:options:) or init(imageURL:options:). These initializers create a CIFilter object with an outputImage which is a CIImage representation of the supplied RAW image. You can process After calling this method, the `CIFilter` object returns a CIImage object that’s properly processed similar to images retrieved using the `outputImage` key.

Important

Core Image doesn’t process the supplied RAW image until the filter’s outputImage is rendered. For this reason, if you supply this initializer with a RAW image of an unsupported format, the filter object will be initialized but its `outputImage` will be `nil`.

## See Also

### Deprecated

init!(cvPixelBuffer: CVPixelBuffer!, properties: [AnyHashable : Any]!, options: [CIRAWFilterOption : Any]!)

Creates a filter from a Core Video pixel buffer.

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

class func supportedRawCameraModels() -> [String]!Deprecated

