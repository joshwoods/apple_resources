

- ARKit
- ARReferenceImage
-  init(\_:orientation:physicalWidth:) 

Initializer

# init(\_:orientation:physicalWidth:)

Creates a new reference image from a Core Video pixel buffer.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
init(
    _ pixelBuffer: CVPixelBuffer,
    orientation: CGImagePropertyOrientation,
    physicalWidth: CGFloat
)
```

## Parameters 

`pixelBuffer`  

A Core Video pixel buffer containing the image data for the new image.

`orientation`  

The intended display orientation for the image.

`physicalWidth`  

The real-world width, in meters, of the image.

## Discussion

To accurately recognize the position and orientation of an image in the AR environment, ARKit must know the image’s physical size. When you call this initializer, ARKit uses the `physicalWidth` measurement and `orientation` you provide together with the aspect ratio of the image itself to calculate the physical height. Use the physicalSize property of the created ARReferenceImage object to retrieve these values.

Important

ARKit preprocesses reference images before using them for image detection. To provide reference images bundled with your app, create AR reference image assets in your Xcode asset catalog, and use the referenceImages(inGroupNamed:bundle:) method to load them.

## See Also

### Creating Reference Images

init(CGImage, orientation: CGImagePropertyOrientation, physicalWidth: CGFloat)

Creates a new reference image from a Core Graphics image object.

