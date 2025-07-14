

- Core Image
- Tile Effect Filters
-  twelvefoldReflectedTile() 

Type Method

# twelvefoldReflectedTile()

Creates a tiled image by rotating in increments of 30 degrees.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func twelvefoldReflectedTile() -> any CIFilter & CITwelvefoldReflectedTile
```

## Return Value

The tiled image.

## Discussion

This method applies the 12-fold reflected tile filter to an image. The effect produces a 12-way reflected tile image.

The 12-fold reflected tile filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`angle`  
A `float` representing the direction of distortion, in radians as an NSNumber.

`width`  
A `float` representing the set width of each tile as an `NSNumber`.

The following code creates a filter that results in a 12-fold pattern angled at 30 degrees and then repeated:

func twelveFoldReflected(inputImage: CIImage) -> CIImage {
    let twelveFoldReflectedTile = CIFilter.twelvefoldReflectedTile()
    twelveFoldReflectedTile.inputImage = inputImage
    twelveFoldReflectedTile.center = CGPoint(x: 150, y: 150)
    twelveFoldReflectedTile.angle = 0
    twelveFoldReflectedTile.width = 100
    return twelveFoldReflectedTile.outputImage!
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

class func triangleKaleidoscope() -> any CIFilter &amp; CITriangleKaleidoscope

Create a triangular kaleidoscope effect and then tiles the result.

class func triangleTile() -> any CIFilter &amp; CITriangleTile

Tiles a triangular area of an image.

