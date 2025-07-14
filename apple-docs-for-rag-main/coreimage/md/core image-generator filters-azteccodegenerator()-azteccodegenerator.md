

- Core Image
- Generator Filters
-  aztecCodeGenerator() 

Type Method

# aztecCodeGenerator()

Generates a low-density barcode.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func aztecCodeGenerator() -> any CIFilter & CIAztecCodeGenerator
```

## Return Value

The generated image.

## Discussion

This method generates an Aztec code as an image. The Aztec barcode code is a low-density barcode defined in the ISO/IEC 24778:2008 standard. This code is commonly used for transport ticketing or boarding passes.

The Aztec code generator filter uses the following properties:

`message`  
The data to be encoded as an Aztec code. An NSData object whose display name is Message.

`correctionLevel`  
A `float` representing the percentage of redundancy to add to the message data. A higher correction level allows the barcode to be correctly read even when partially damaged.

`layers`  
A `float` representing the number of concentric squares encoding the barcode data. When the value is zero, Core Image automatically determines the appropriate number of layers to encode the message data at the specified correction level.

`compactStyle`  
A `float` determining the use of compact or full-size Aztec barcode format. The compact format can store up to 44 bytes of message data in up to 4 layers. The full-size format can store up to 1914 bytes of message data in up to 32 layers. Leave unset, or set to 0 for automatic.

The following code creates a filter that generates an Aztec barcode:

func aztecCode(inputMessage: String) -> CIImage {
    let aztecCodeGenerator = CIFilter.aztecCodeGenerator()
    aztecCodeGenerator.correctionLevel = 15
    aztecCodeGenerator.compactStyle = 0
    aztecCodeGenerator.message = inputMessage.data(using: .ascii)!
    aztecCodeGenerator.layers = 10
    return aztecCodeGenerator.outputImage!
}

## See Also

### Filters

class func attributedTextImageGenerator() -> any CIFilter &amp; CIAttributedTextImageGenerator

Generates an attributed-text image.

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

