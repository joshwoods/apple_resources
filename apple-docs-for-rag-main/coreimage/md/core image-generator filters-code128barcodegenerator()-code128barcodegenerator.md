

- Core Image
- Generator Filters
-  code128BarcodeGenerator() 

Type Method

# code128BarcodeGenerator()

Generates a high-density, linear barcode.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func code128BarcodeGenerator() -> any CIFilter & CICode128BarcodeGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a Code 128 barcode as an image. Code 128 is a high-density linear barcode defined in the ISO/IEC 15417:2007 standard. Use this filter to generate alphanumeric or numeric-only barcodes. The barcode can contain any of the 128 ASCII characters.

The Code 128 barcode filter uses the following properties:

`message`  
NSData containing the message to encode in the Code 128 barcode.

`quietSpace`  
NSNumber containing the number of empty white pixels that should surround the barcode.

`barcodeHeight`  
`NSNumber` containing the height of the generated barcode in pixels.

The following code creates a filter that generates a Code 128 barcode:

func code128Barcode(barcode: String) -> CIImage {
    let code128Barcode = CIFilter.code128BarcodeGenerator()
    code128Barcode.message = barcode.data(using: .ascii)!
    code128Barcode.quietSpace = 5
    code128Barcode.barcodeHeight = 20
    return code128Barcode.outputImage!
}

## See Also

### Filters

class func attributedTextImageGenerator() -> any CIFilter &amp; CIAttributedTextImageGenerator

Generates an attributed-text image.

class func aztecCodeGenerator() -> any CIFilter &amp; CIAztecCodeGenerator

Generates a low-density barcode.

class func barcodeGenerator() -> any CIFilter &amp; CIBarcodeGenerator

Generates a barcode as an image from the descriptor.

class func blurredRectangleGenerator() -> any CIFilter &amp; CIBlurredRectangleGenerator

Generates a blurred rectangle.

class func checkerboardGenerator() -> any CIFilter &amp; CICheckerboardGenerator

Generates a checkerboard image.

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

