

- Core Image
- CIContext
-  draw(\_:in:from:) 

Instance Method

# draw(\_:in:from:)

Renders a region of an image to a rectangle in the context destination.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func draw(
    _ image: CIImage,
    in inRect: CGRect,
    from fromRect: CGRect
)
```

## Parameters 

`im`  

A Core Image image object.

`dest`  

The rectangle in the context destination to draw into. The image is scaled to fill the destination rectangle.

`src`  

The subregion of the image that you want to draw into the context, with the origin and target size defined by the `dest` parameter. This rectangle is always in pixel dimensions.

## Discussion

In iOS, this method draws the `CIImage` object into a renderbuffer for the OpenGL ES context. Use this method only if the `CIContext` object is created with `contextWithEAGLContext:` and if you are rendering to a CAEAGLayer. This method is asynchronous for apps linked against the iOS 6 or later SDK.

In macOS, you need to be aware of whether the `CIContext` object is created with a `CGContextRef` or a `CGLContext` object. If you create the `CIContext` object with a `CGContextRef`, the dimensions of the destination rectangle are in points. If you create the `CIContext` object with a `CGLContext` object, the dimensions are in pixels.

## See Also

### Drawing Images

func draw(CIImage, at: CGPoint, from: CGRect)

Renders a region of an image to a point in the context destination.

