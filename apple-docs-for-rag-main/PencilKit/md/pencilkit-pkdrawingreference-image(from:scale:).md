

- PencilKit
- PKDrawingReference
-  image(from:scale:) 

Instance Method

# image(from:scale:)

Returns an image object that contains the specified portion of the drawing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func image(
    from rect: CGRect,
    scale: CGFloat
) -> UIImage
```

**macOS**

``` source
func image(
    from rect: CGRect,
    scale: CGFloat
) -> NSImage
```

## Parameters 

`rect`  

The portion of the drawing that you want to capture. Specify a rectangle in the canvas’ coordinate system.

`scale`  

The scale factor at which to create the image. Specifying scale factors greater than `1.0` creates an image with more detail. For example, you might specify a scale factor of `2.0` or `3.0` when displaying the image on a Retina display.

## Return Value

A new image object that contains the rendered content.

## Discussion

This method creates a new image and renders content from the canvas into that image at the specified scale factor.

