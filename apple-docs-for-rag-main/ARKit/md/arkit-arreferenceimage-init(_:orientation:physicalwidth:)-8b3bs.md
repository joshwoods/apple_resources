

- ARKit
- ARReferenceImage
-  init(\_:orientation:physicalWidth:) 

Initializer

# init(\_:orientation:physicalWidth:)

Creates a new reference image from a Core Graphics image object.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
init(
    _ image: CGImage,
    orientation: CGImagePropertyOrientation,
    physicalWidth: CGFloat
)
```

## Parameters 

`image`  

A Core Graphics image object.

`orientation`  

The intended display orientation for the image.

`physicalWidth`  

The real-world width, in meters, of the image.

## Discussion

To accurately recognize the position and orientation of an image in the AR environment, ARKit must know the image’s physical size. When you call this initializer, ARKit uses the `physicalWidth` measurement and `orientation` you provide together with the aspect ratio of the image itself to calculate the physical height. Use the physicalSize property of the created ARReferenceImage object to retrieve these values.

Important

ARKit preprocesses reference images before using them for image detection. To provide reference images bundled with your app, create AR Reference Image assets in your Xcode asset catalog, and use the `referenceImageSetNamed(_:in:)` method to load them.

## See Also

### Creating Reference Images

init(CVPixelBuffer, orientation: CGImagePropertyOrientation, physicalWidth: CGFloat)

Creates a new reference image from a Core Video pixel buffer.

