

- SwiftUI
- GraphicsContext
-  resolveSymbol(id:) 

Instance Method

# resolveSymbol(id:)

Gets the identified child view as a resolved symbol, if the view exists.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func resolveSymbol(id: ID) -> GraphicsContext.ResolvedSymbol? where ID : Hashable
```

## Parameters 

`id`  

The value that you used to tag the view when you define it in the `symbols` parameter of the Canvas initializer init(opaque:colorMode:rendersAsynchronously:renderer:symbols:).

## Return Value

The resolved symbol, or `nil` if SwiftUI can’t find a child view with the given `id`.

## See Also

### Resolving a drawn entity

func resolve(_:)

Gets a version of an image that’s fixed with the current values of the graphics context’s environment.

struct ResolvedSymbol

A static sequence of drawing operations that may be drawn multiple times, preserving their resolution independence.

struct ResolvedImage

An image resolved to a particular environment.

struct ResolvedText

A text view resolved to a particular environment.

