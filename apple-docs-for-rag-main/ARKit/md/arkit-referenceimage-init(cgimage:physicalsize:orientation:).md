

- ARKit
- ReferenceImage
-  init(cgimage:physicalSize:orientation:) 

Initializer

# init(cgimage:physicalSize:orientation:)

Creates a reference image from a Core Graphics image.

visionOS 1.0+

``` source
init(
    cgimage: CGImage,
    physicalSize: CGSize,
    orientation: CGImagePropertyOrientation = .up
)
```

## Parameters 

`cgimage`  

The image to use as a reference during tracking.

`physicalSize`  

The size of the image in meters.

`orientation`  

The orientation of the image asset.

## See Also

### Creating a reference image

init(pixelBuffer: CVPixelBuffer, physicalSize: CGSize, orientation: CGImagePropertyOrientation)

Creates a reference image from a pixel buffer.

static func loadReferenceImages(inGroupNamed: String, bundle: Bundle?) -> [ReferenceImage]

Creates multiple reference images based on their group name in an asset catalog.

