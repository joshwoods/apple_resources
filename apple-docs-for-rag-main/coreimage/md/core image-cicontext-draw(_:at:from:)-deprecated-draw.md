

- Core Image
- CIContext
-  draw(\_:at:from:) Deprecated

Instance Method

# draw(\_:at:from:)

Renders a region of an image to a point in the context destination.

iOS 5.0–6.0DeprecatediPadOS 5.0–6.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.8DeprecatedtvOS 9.0+visionOS 1.0–1.0Deprecated

``` source
func draw(
    _ image: CIImage,
    at atPoint: CGPoint,
    from fromRect: CGRect
)
```

Deprecated

Instead use draw(_:in:from:).

## Parameters 

`im`  

A Core Image image object.

`p`  

The point in the context destination to draw to.

`src`  

The region of the image to draw.

## Discussion

This method because it is ambiguous as to the units of the dimensions and won’t work as expected in a high-resolution environment which is why you should use `drawImage:inRect:fromRect:` instead.

On iOS platforms, this method draws the image onto a render buffer for the OpenGL ES context. Use this method only if the `CIContext` object is created with `contextWithEAGLContext:`, and hence, you are rendering to a CAEAGLLayer.

## See Also

### Drawing Images

func draw(CIImage, in: CGRect, from: CGRect)

Renders a region of an image to a rectangle in the context destination.

