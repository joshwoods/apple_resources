

- Core Image
- Generator Filters
-  checkerboardGenerator() 

Type Method

# checkerboardGenerator()

Generates a checkerboard image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func checkerboardGenerator() -> any CIFilter & CICheckerboardGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a checkerboard pattern as an image. The effect requires the size, sharpness, and color properties to create the pattern.

The checkerboard generator filter uses the following properties:

`center`  
A `vector` representing the center of the image as a CIVector.

`color0`  
A CIColor representing the first color of the pattern.

`color1`  
A `CIColor` representing the second color of the pattern.

`sharpness`  
A `float` representing the sharpness of the pattern as an NSNumber.

`width`  
A `float` representing the width of the checkerboard squares as an `NSNumber`.

The following code creates a filter that generates a black-and-white checkered pattern:

func checkerBoard() -> CIImage {
    let checkerBoardGenerator = CIFilter.checkerboardGenerator()
    checkerBoardGenerator.setDefaults()
    checkerBoardGenerator.center = CGPoint(x: 0, y: 0)
    checkerBoardGenerator.color0 = .white
    checkerBoardGenerator.color1 = .black
    checkerBoardGenerator.width = 40
    checkerBoardGenerator.sharpness = 1
    return checkerBoardGenerator.outputImage!
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

