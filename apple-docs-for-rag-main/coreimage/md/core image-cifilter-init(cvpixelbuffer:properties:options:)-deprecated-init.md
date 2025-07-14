

- Core Image
- CIFilter
-  init(cvPixelBuffer:properties:options:) Deprecated

Initializer

# init(cvPixelBuffer:properties:options:)

Creates a filter from a Core Video pixel buffer.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init!(
    cvPixelBuffer pixelBuffer: CVPixelBuffer!,
    properties: [AnyHashable : Any]!,
    options: [CIRAWFilterOption : Any]! = [:]
)
```

Deprecated

Use init(cvPixelBuffer:properties:) instead.

## Parameters 

`pixelBuffer`  

CVPixelBufferRef with one of the following RAW pixel format types:

kCVPixelFormatType_14Bayer_GRBG

kCVPixelFormatType_14Bayer_RGGB

kCVPixelFormatType_14Bayer_BGGR

kCVPixelFormatType_14Bayer_GBRG

`properties`  

A properties dictionary. Defines the properties of the pixel buffer.

`options`  

An options dictionary. You can pass any of the keys defined in RAW Image Options.

## Return Value

A CIFilter object.

## Discussion

The first step when working with RAW images in Core Image is to process the image using either init(imageData:options:) or init(imageURL:options:). These initializers create a CIFilter object with an outputImage which is a CIImage representation of the supplied RAW image.

Important

Core Image doesn't process the supplied RAW image until the filter's outputImage is rendered. For this reason, if you supply this initializer with a RAW image of an unsupported format, the filter object will be initialized but its outputImage will be nil.

## See Also

### Deprecated

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

class func supportedRawCameraModels() -> [String]!Deprecated

