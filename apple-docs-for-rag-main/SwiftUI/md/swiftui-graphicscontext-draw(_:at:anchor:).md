

- SwiftUI
- GraphicsContext
-  draw(\_:at:anchor:) 

Instance Method

# draw(\_:at:anchor:)

Draws a resolved image into the context, aligning an anchor within the image to a point in the context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func draw(
    _ image: GraphicsContext.ResolvedImage,
    at point: CGPoint,
    anchor: UnitPoint = .center
)
```

Show all declarations

## Parameters 

`image`  

The GraphicsContext.ResolvedImage to draw. Get a resolved image from an Image by calling resolve(_:). Alternatively, you can call draw(_:at:anchor:) with an Image, and that method performs the resolution automatically.

`point`  

A point within the rectangle of the resolved image to anchor to a point in the context.

`anchor`  

A UnitPoint within the context to align the image with. The default is center.

## Discussion

The current context state defines the full drawing operation. For example, the current transformation and clip shapes affect how SwiftUI draws the image.

## See Also

### Drawing images, text, and views

func draw(_:in:)

Draws a resolved symbol into the context, using the specified rectangle as a layout frame.

func draw(_:in:style:)

Draws a resolved image into the context, using the specified rectangle as a layout frame.

