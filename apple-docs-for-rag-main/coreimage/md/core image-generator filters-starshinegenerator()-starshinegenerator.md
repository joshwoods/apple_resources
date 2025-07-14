

- Core Image
- Generator Filters
-  starShineGenerator() 

Type Method

# starShineGenerator()

Generates a star-shine image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func starShineGenerator() -> any CIFilter & CIStarShineGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a star-shine image. The effect is similar to a supernova effect. You can use this filter to simulate a lens flare.

The star-shine generator filter uses the following properties:

`center`  
A `vector` representing the center of the flare as a CGPoint.

`color`  
A color representing the color of the flare as a CGColor.

`radius`  
A `float` representing the radius of the flare as an NSNumber.

`crossScale`  
A `float` representing the cross flare size relative to the round central flare as an `NSNumber`.

`crossAngle`  
A `float` representing the angle of the flare as an `NSNumber`.

`crossOpacity`  
A `float` representing the thickness of the cross opacity as an `NSNumber`.

`crossWidth`  
A `float` representing the cross width as an `NSNumber`.

`epsilon`  
A `float` representing the epsilon as an `NSNumber`.

The following code generates a star-shaped silhouette with a black background.

func starShine() -> CIImage {
    let starShineGenerator = CIFilter.starShineGenerator()
    starShineGenerator.center = CGPoint(x: 150, y: 150)
    starShineGenerator.color = .green
    starShineGenerator.radius = 50
    starShineGenerator.crossScale = 15
    starShineGenerator.crossAngle = 0.60
    starShineGenerator.crossOpacity = -2
    starShineGenerator.crossWidth = 2.5
    starShineGenerator.epsilon = -2.0
    return starShineGenerator.outputImage!
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

class func roundedRectangleStrokeGenerator() -> any CIFilter &amp; CIRoundedRectangleStrokeGenerator

Creates an image containing the outline of a rounded rectangle.

class func stripesGenerator() -> any CIFilter &amp; CIStripesGenerator

Generates a line of stripes as an image

class func sunbeamsGenerator() -> any CIFilter &amp; CISunbeamsGenerator

Generates an image resembling the sun.

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

