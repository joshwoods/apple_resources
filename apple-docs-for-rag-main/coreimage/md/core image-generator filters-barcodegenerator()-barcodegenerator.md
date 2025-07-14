

- Core Image
- Generator Filters
-  barcodeGenerator() 

Type Method

# barcodeGenerator()

Generates a barcode as an image from the descriptor.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func barcodeGenerator() -> any CIFilter & CIBarcodeGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a custom barcode as an image. The effect uses barcode descriptors to specify properties of the generated barcode.

The barcode generator uses the following property:

`barcodeDescriptor`  
An instance of CIBarcodeDescriptor with the input parameters supplied.

The following code creates a filter that generates a QR code containing the text *Johnny Appleseed.*

func barcode(inputMessage: Data) -> CIImage {
   let barcodeGenerator = CIFilter.barcodeGenerator()
    barcodeGenerator.barcodeDescriptor = CIQRCodeDescriptor(payload: inputMessage, symbolVersion: 1, maskPattern: 4, errorCorrectionLevel: .levelL)!
    return barcodeGenerator.outputImage!
}

let johnnyAppleseed: [UInt8] = [0x41, 0x04, 0xA6, 0xF6, 0x86, 0xE6, 0xE7, 0x92, 0x04, 0x17, 0x07, 0x06, 0xC6, 0x57, 0x36, 0x56, 0x56, 0x40, 0xEC]
let data = Data(johnnyAppleseed)

let bImage = barcode(inputMessage: data)

## See Also

### Filters

class func attributedTextImageGenerator() -> any CIFilter &amp; CIAttributedTextImageGenerator

Generates an attributed-text image.

class func aztecCodeGenerator() -> any CIFilter &amp; CIAztecCodeGenerator

Generates a low-density barcode.

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

### Related Documentation

class CIAztecCodeDescriptor

A concrete subclass of that represents an Aztec code symbol.

class CIDataMatrixCodeDescriptor

A concrete subclass of that represents a Data Matrix code symbol.

class CIPDF417CodeDescriptor

A concrete subclass of that represents a PDF417 symbol.

class CIQRCodeDescriptor

A concrete subclass of that represents a square QR code symbol.

