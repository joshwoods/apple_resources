

- Core Image
- Generator Filters
-  roundedRectangleStrokeGenerator() 

Type Method

# roundedRectangleStrokeGenerator()

Creates an image containing the outline of a rounded rectangle.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.5+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class func roundedRectangleStrokeGenerator() -> any CIFilter & CIRoundedRectangleStrokeGenerator
```

## Return Value

A CIImage containing the stroked rectangle.

## Discussion

This filter creates an outline of a rounded rectangle.

The filter takes the following properties:

`extent`  
A CGRect containing the position and size of the rectangle.

`width`  
The width of the stroke to draw.

`radius`  
The corner radius.

The following code generates an image containing a stroked rounded rectangle:

func roundedRectangleStroke() -> CIImage {
    let filter = CIFilter.roundedRectangleStrokeGenerator()
    filter.extent = CGRect(x: 0, y: 0, width: 200, height: 100)
    filter.color = CIColor.red
    filter.width = 5
    filter.radius = 20
    return filter.outputImage!
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

class func roundedRectangleGenerator() -> any CIFilter &amp; CIRoundedRectangleGenerator

Generates a rounded rectangle image.

class func starShineGenerator() -> any CIFilter &amp; CIStarShineGenerator

Generates a star-shine image.

class func stripesGenerator() -> any CIFilter &amp; CIStripesGenerator

Generates a line of stripes as an image

class func sunbeamsGenerator() -> any CIFilter &amp; CISunbeamsGenerator

Generates an image resembling the sun.

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

