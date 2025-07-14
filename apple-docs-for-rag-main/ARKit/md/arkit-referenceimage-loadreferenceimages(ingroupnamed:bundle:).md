

- ARKit
- ReferenceImage
-  loadReferenceImages(inGroupNamed:bundle:) 

Type Method

# loadReferenceImages(inGroupNamed:bundle:)

Creates multiple reference images based on their group name in an asset catalog.

visionOS 1.0+

``` source
static func loadReferenceImages(
    inGroupNamed groupName: String,
    bundle: Bundle? = nil
) -> [ReferenceImage]
```

## Parameters 

`groupName`  

The name of the group of assets in an asset catalog.

`bundle`  

The bundle that contains the image assets. If `nil`, this method loads reference images from the main bundle.

## Return Value

An array of reference images loaded from the group you specify.

## See Also

### Creating a reference image

init(cgimage: CGImage, physicalSize: CGSize, orientation: CGImagePropertyOrientation)

Creates a reference image from a Core Graphics image.

init(pixelBuffer: CVPixelBuffer, physicalSize: CGSize, orientation: CGImagePropertyOrientation)

Creates a reference image from a pixel buffer.

