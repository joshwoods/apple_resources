

- Core Image
- CIImage
-  draw(in:from:operation:fraction:) 

Instance Method

# draw(in:from:operation:fraction:)

Draws all or part of the image in the specified rectangle in the current coordinate system

macOS 10.4+

``` source
func draw(
    in rect: NSRect,
    from fromRect: NSRect,
    operation op: NSCompositingOperation,
    fraction delta: CGFloat
)
```

## Parameters 

`dstRect`  

The rectangle in which to draw the image.

`srcRect`  

The source rectangle specifying the portion of the image you want to draw. The coordinates of this rectangle must be specified using the image's own coordinate system.

`op`  

The compositing operation to use when drawing the image. For details, see NSCompositingOperation.

`delta`  

The opacity of the image, specified as a value from `0.0` to `1.0`. Specifying a value of `0.0` draws the image as fully transparent while a value of `1.0` draws the image as fully opaque. Values greater than `1.0` are interpreted as `1.0`.

## Discussion

If the `srcRect` and `dstRect` rectangles have different sizes, the source portion of the image is scaled to fit the specified destination rectangle. The image is otherwise positioned and oriented using the current coordinate system.

## See Also

### Drawing Images

func draw(at: NSPoint, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image at the specified point in the current coordinate system.

