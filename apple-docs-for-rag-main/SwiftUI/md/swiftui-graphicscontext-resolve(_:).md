

- SwiftUI
- GraphicsContext
-  resolve(\_:) 

Instance Method

# resolve(\_:)

Gets a version of an image that’s fixed with the current values of the graphics context’s environment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func resolve(_ image: Image) -> GraphicsContext.ResolvedImage
```

Show all declarations

## Parameters 

`image`  

The Image to resolve.

## Return Value

An image that’s resolved into the current context’s environment, taking into account environment values like the display resolution and current color scheme.

## Discussion

You can measure the resolved image by looking at its size and baseline properties. You can draw the resolved image with the context’s draw(_:in:style:) or draw(_:at:anchor:) method.

## See Also

### Resolving a drawn entity

func resolveSymbol&lt;ID>(id: ID) -> GraphicsContext.ResolvedSymbol?

Gets the identified child view as a resolved symbol, if the view exists.

struct ResolvedSymbol

A static sequence of drawing operations that may be drawn multiple times, preserving their resolution independence.

struct ResolvedImage

An image resolved to a particular environment.

struct ResolvedText

A text view resolved to a particular environment.

