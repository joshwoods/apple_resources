

- Core Image
- Generator Filters
-  attributedTextImageGenerator() 

Type Method

# attributedTextImageGenerator()

Generates an attributed-text image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func attributedTextImageGenerator() -> any CIFilter & CIAttributedTextImageGenerator
```

## Return Value

The generated image.

## Discussion

This method generates an attributed-text image. The effect takes the input string property and the scale factor to scale up the text. You commonly combine this filter with other filters to create a watermark on images.

The attributed-text image generator filter uses the following properties:

`text`  
An NSAttributedString.

`scaleFactor`  
A `float` representing the scale of the font to use for the generated text.

padding  
A `float` representing the value for an additional number of pixels to pad around the text’s bounding box.

The following code creates a filter that generates an attributed-text image:

func attributedTextImage() -> CIImage {
    let attributedTextImageFilter = CIFilter.attributedTextImageGenerator()
    attributedTextImageFilter.text = NSAttributedString(string: &quot;Hello world! 👋&quot;)
    attributedTextImageFilter.scaleFactor = 10
    attributedTextImageFilter.padding = 5
    return attributedTextImageFilter.outputImage!
}

## See Also

### Filters

class func aztecCodeGenerator() -> any CIFilter &amp; CIAztecCodeGenerator

Generates a low-density barcode.

class func barcodeGenerator() -> any CIFilter &amp; CIBarcodeGenerator

Generates a barcode as an image from the descriptor.

class func blurredRectangleGenerator() -> any CIFilter &amp; CIBlurredRectangleGenerator

Generates a blurred rectangle.

class func checkerboardGenerator() -> any CIFilter &amp; CICheckerboardGenerator

Generates a checkerboard image.

class func code128BarcodeGenerator() -> any CIFilter &amp; CICode128BarcodeGenerator

Generates a high-density, linear barcode.

class func lenticularHaloGenerator() -> any CIFilter &amp; CILenticularHaloGenerator

Generates a lenticular halo image.

class func meshGenerator() -> any CIFilter &amp; CIMeshGenerator

Generates a pattern made from an array of line segments.

class func pdf417BarcodeGenerator() -> any CIFilter &amp; CIPDF417BarcodeGenerator

Generates a high-density linear barcode.

class func qrCodeGenerator() -> any CIFilter &amp; CIQRCodeGenerator

Generates a quick response (QR) code image.

class func randomGenerator() -> any CIFilter &amp; CIRandomGenerator

Generates a random filter image.

class func roundedRectangleGenerator() -> any CIFilter &amp; CIRoundedRectangleGenerator

Generates a rounded rectangle image.

class func roundedRectangleStrokeGenerator() -> any CIFilter &amp; CIRoundedRectangleStrokeGenerator

Creates an image containing the outline of a rounded rectangle.

class func starShineGenerator() -> any CIFilter &amp; CIStarShineGenerator

Generates a star-shine image.

class func stripesGenerator() -> any CIFilter &amp; CIStripesGenerator

Generates a line of stripes as an image

class func sunbeamsGenerator() -> any CIFilter &amp; CISunbeamsGenerator

Generates an image resembling the sun.

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

