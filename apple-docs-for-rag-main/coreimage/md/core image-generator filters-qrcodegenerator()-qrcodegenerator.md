

- Core Image
- Generator Filters
-  qrCodeGenerator() 

Type Method

# qrCodeGenerator()

Generates a quick response (QR) code image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func qrCodeGenerator() -> any CIFilter & CIQRCodeGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a QR code as an image. QR codes are a high-density matrix barcode format defined in the ISO/IEC 18004:2006 standard.

The QR code generator filter uses the following properties:

`message`  
A `string` representing the data to be encoded as a QR Code as NSData.

`correctionLevel`  
A single letter `string` representing the error-correction format as an NSString. L is 7 precent correction, M is 15 precent correction, Q is 25 precent correction, and H is 30 precent correction.

The following code creates a filter that generates a QR code:

func qrCode(inputMessage: String) -> CIImage {
    let qrCodeGenerator = CIFilter.qrCodeGenerator()
    qrCodeGenerator.message = inputMessage.data(using: .ascii)!
    qrCodeGenerator.correctionLevel = &quot;H&quot;
    return qrCodeGenerator.outputImage!
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

class func code128BarcodeGenerator() -> any CIFilter &amp; CICode128BarcodeGenerator

Generates a high-density, linear barcode.

class func lenticularHaloGenerator() -> any CIFilter &amp; CILenticularHaloGenerator

Generates a lenticular halo image.

class func meshGenerator() -> any CIFilter &amp; CIMeshGenerator

Generates a pattern made from an array of line segments.

class func pdf417BarcodeGenerator() -> any CIFilter &amp; CIPDF417BarcodeGenerator

Generates a high-density linear barcode.

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

