

- Core Image
- CIFilter
-  init(imageURL:options:) Deprecated

Initializer

# init(imageURL:options:)

Creates a filter that allows the processing of RAW images.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init!(
    imageURL url: URL!,
    options: [CIRAWFilterOption : Any]! = [:]
)
```

Deprecated

Use init(imageURL:) instead.

## Parameters 

`url`  

The location of a RAW image file.

`options`  

An options dictionary. You can pass any of the keys defined in RAW Image Options.

## Return Value

A `CIFilter` object.

## Discussion

The first step when working with RAW images in Core Image is to process the image using either init(imageData:options:) or init(imageURL:options:). These initializers create a CIFilter object with an outputImage which is a CIImage representation of the supplied RAW image.

The newly created filter object allows you fine control over the image processing that isn’t available when working with processed images such a JPEG. The following listing shows how to create a Core Image filter based on a URL named `imageURL`. The image is processed so that its neutral temperature is set to 2,000 Kelvin (giving a blue tint) and its baseline exposure doubled. Finally, a Core Image vignette filter is applied to the processed image in the same way it would be with any other source image:

let rawFilter = CIFilter(imageURL: imageURL, options: nil)
rawFilter?.setValue(2000,    
                    forKey: kCIInputNeutralTemperatureKey)
if let baselineExposure = rawFilter?.value(forKey: kCIInputBaselineExposureKey) as? NSNumber {    
    rawFilter?.setValue(baselineExposure.doubleValue * 2.5,                        forKey: kCIInputBaselineExposureKey)
}
let vignettedImage = rawFilter?.outputImage?.applyingFilter(    
    &quot;CIVignette&quot;,    
    withInputParameters: [kCIInputIntensityKey: 5])
if let outputImage = vignettedImage {    
    imageView.image = UIImage(ciImage: outputImage)
}

Listing 1 Processing a RAW image.

Important

Core Image doesn’t process the supplied RAW image until the filter’s outputImage is rendered. For this reason, if you supply this initializer with a RAW image of an unsupported format, the filter object will be initialized but its `outputImage` will be `nil`.

## See Also

### Deprecated

init!(cvPixelBuffer: CVPixelBuffer!, properties: [AnyHashable : Any]!, options: [CIRAWFilterOption : Any]!)

Creates a filter from a Core Video pixel buffer.

Deprecated

init!(imageData: Data!, options: [CIRAWFilterOption : Any]!)

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

