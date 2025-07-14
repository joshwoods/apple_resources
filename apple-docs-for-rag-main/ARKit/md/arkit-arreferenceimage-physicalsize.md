

- ARKit
- ARReferenceImage
-  physicalSize 

Instance Property

# physicalSize

The real-world dimensions, in meters, of the image.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var physicalSize: CGSize { get }
```

## Discussion

To accurately recognize the position and orientation of an image in the AR environment, ARKit must know the image’s physical size. You provide this information when creating an AR reference image in your Xcode project’s asset catalog, or when programmatically creating an ARReferenceImage.

When you want to recognize different-sized versions of a reference image, you set automaticImageScaleEstimationEnabled to true, and in this case, ARKit disregards `physicalSize`.

## See Also

### Examining a Reference Image

var name: String?

A descriptive name for the image.

var resourceGroupName: String?

The AR resource group name for this image.

