

- Core Image
- Tile Effect Filters
-  triangleKaleidoscope() 

Type Method

# triangleKaleidoscope()

Create a triangular kaleidoscope effect and then tiles the result.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func triangleKaleidoscope() -> any CIFilter & CITriangleKaleidoscope
```

## Return Value

The tiled image.

## Discussion

This method applies the triangle kaleidoscope filter to an image. The effect produces a complex tiled pattern from a triangular area input image.

The triangle kaleidoscope tile filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`decay`  
A `float` representing the intensity of the color fade from the the center of the triangle as an NSNumber.

`point`  
A set of coordinates marking the center of the triangular area of the input image as a CIVector.

`rotation`  
A `float` representing the angle of rotation of the triangle as an `NSNumber`.

`size`  
A `float` representing the size in pixels of the triangle as an `NSNumber`.

The following code creates a filter that produces a triangle tile of the input image, creating an optical illusion:

func triangleKaleidoscope(inputImage: CIImage) -> CIImage {
    let triangleKaleidoscopeTile = CIFilter.triangleKaleidoscope()
    triangleKaleidoscopeTile.inputImage = inputImage
    triangleKaleidoscopeTile.point = CGPoint(x: 150, y: 150)
    triangleKaleidoscopeTile.size = 700
    triangleKaleidoscopeTile.rotation = -0.36
    triangleKaleidoscopeTile.decay = 0.85
    return triangleKaleidoscopeTile.outputImage!
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

class func kaleidoscope() -> any CIFilter &amp; CIKaleidoscope

Creates a 12-way kaleidoscopic image from an image.

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

class func triangleTile() -> any CIFilter &amp; CITriangleTile

Tiles a triangular area of an image.

class func twelvefoldReflectedTile() -> any CIFilter &amp; CITwelvefoldReflectedTile

Creates a tiled image by rotating in increments of 30 degrees.

