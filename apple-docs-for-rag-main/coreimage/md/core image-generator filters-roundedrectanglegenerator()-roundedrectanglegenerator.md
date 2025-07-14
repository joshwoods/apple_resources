

- Core Image
- Generator Filters
-  roundedRectangleGenerator() 

Type Method

# roundedRectangleGenerator()

Generates a rounded rectangle image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func roundedRectangleGenerator() -> any CIFilter & CIRoundedRectangleGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a rounded rectangle image with the specified size, corner radius, and color properties.

The rounded rectangle generator filter uses the following properties:

`color`  
A CIColor representing the color of the rounded rectangle.

`extent`  
A CGRect representing the size of the rounded rectangle.

`radius`  
A `float` representing the curve of the rectangle’s corners.

The following code creates a filter that generates a light blue square with rounded corners:

func roundedRectangle () -> CIImage {
    let roundedRectangleGenerator = CIFilter.roundedRectangleGenerator()
    roundedRectangleGenerator.color = CIColor(red: 96/255, green: 173/255, blue: 193/255)
    roundedRectangleGenerator.extent = CGRect(x: 0, y: 1, width: 700, height: 700)
    roundedRectangleGenerator.radius = 100
    return roundedRectangleGenerator.outputImage!
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

class func qrCodeGenerator() -> any CIFilter &amp; CIQRCodeGenerator

Generates a quick response (QR) code image.

class func randomGenerator() -> any CIFilter &amp; CIRandomGenerator

Generates a random filter image.

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

