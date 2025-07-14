

- SwiftUI
- GraphicsContext
-  draw(\_:in:) 

Instance Method

# draw(\_:in:)

Draws a resolved symbol into the context, using the specified rectangle as a layout frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func draw(
    _ symbol: GraphicsContext.ResolvedSymbol,
    in rect: CGRect
)
```

Show all declarations

## Parameters 

`symbol`  

The GraphicsContext.ResolvedSymbol to draw. Get a resolved symbol by calling resolveSymbol(id:) with the identifier that you use to tag the corresponding child view during Canvas initialization.

`rect`  

The rectangle in the current user space to draw the symbol in.

## Discussion

The current context state defines the full drawing operation. For example, the current transformation and clip shapes affect how SwiftUI draws the symbol.

## See Also

### Drawing images, text, and views

func draw(_:in:style:)

Draws a resolved image into the context, using the specified rectangle as a layout frame.

func draw(_:at:anchor:)

Draws a resolved image into the context, aligning an anchor within the image to a point in the context.

