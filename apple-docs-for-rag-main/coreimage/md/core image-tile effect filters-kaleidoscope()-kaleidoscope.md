

- Core Image
- Tile Effect Filters
-  kaleidoscope() 

Type Method

# kaleidoscope()

Creates a 12-way kaleidoscopic image from an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func kaleidoscope() -> any CIFilter & CIKaleidoscope
```

## Return Value

The tiled image.

## Discussion

This method applies the kaleidoscope tile filter to an image. The effect produces a complex 12-way symmetrical reflected pattern from the input image.

The kaleidoscope tile filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`angle`  
A `float` representing the direction of distortion, in radians as an NSNumber.

`count`  
A `float` representing the number of reflections in the pattern as an `NSNumber`.

The following code creates a filter that results in the creation of a kaleidoscope effect from the input image:

func kaleidoscope(inputImage: CIImage) -> CIImage {
    let kaleidoscopeEffect = CIFilter.kaleidoscope()
    kaleidoscopeEffect.inputImage = inputImage
    kaleidoscopeEffect.count = 6
    kaleidoscopeEffect.center = CGPoint(x: 150, y: 150)
    kaleidoscopeEffect.angle = 0
    return kaleidoscopeEffect.outputImage!
}

## See Also

### Filters

class func affineClamp() -> any CIFilter &amp; CIAffineClamp

Performs a transform on the image and extends the image edges to infinity.

class func affineTile() -> any CIFilter &amp; CIAffineTile

Performs a transform on the image and tiles the result.

class func eightfoldReflectedTile() -> any CIFilter &amp; CIEightfoldReflectedTile

Creates an eight-way reflected pattern.

class func fourfoldReflectedTile() -> any CIFilter &amp; CIFourfoldReflectedTile

Creates a four-way reflected pattern.

class func fourfoldRotatedTile() -> any CIFilter &amp; CIFourfoldRotatedTile

Creates a tiled image by rotating a tile in increments of 90 degrees.

class func fourfoldTranslatedTile() -> any CIFilter &amp; CIFourfoldTranslatedTile

Creates a tiled image by applying four translation operations.

class func glideReflectedTile() -> any CIFilter &amp; CIGlideReflectedTile

Tiles an image by rotating and reflecting a tile from the image.

class func opTile() -> any CIFilter &amp; CIOpTile

Produces an effect that mimics a style of visual art that uses optical illusions.

class func parallelogramTile() -> any CIFilter &amp; CIParallelogramTile

Warps the image to create a parallelogram and tiles the result.

class func perspectiveTile() -> any CIFilter &amp; CIPerspectiveTile

Tiles an image by adjusting the perspective of the image.

class func sixfoldReflectedTile() -> any CIFilter &amp; CISixfoldReflectedTile

Produces a tiled image from a source image by applying a six-way reflected symmetry.

class func sixfoldRotatedTile() -> any CIFilter &amp; CISixfoldRotatedTile

Creates a tiled image by rotating in increments of 60 degrees.

class func triangleKaleidoscope() -> any CIFilter &amp; CITriangleKaleidoscope

Create a triangular kaleidoscope effect and then tiles the result.

class func triangleTile() -> any CIFilter &amp; CITriangleTile

Tiles a triangular area of an image.

class func twelvefoldReflectedTile() -> any CIFilter &amp; CITwelvefoldReflectedTile

Creates a tiled image by rotating in increments of 30 degrees.

