

- SwiftUI
- GraphicsContext
-  GraphicsContext.ResolvedSymbol 

Structure

# GraphicsContext.ResolvedSymbol

A static sequence of drawing operations that may be drawn multiple times, preserving their resolution independence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ResolvedSymbol
```

## Overview

You resolve a child view in preparation for drawing it into a context by calling resolveSymbol(id:). The resolved view takes into account environment values like the display resolution and current color scheme.

## Topics

### Getting the symbol properties

var size: CGSize

The dimensions of the resolved symbol.

## See Also

### Resolving a drawn entity

func resolve(_:)

Gets a version of an image that’s fixed with the current values of the graphics context’s environment.

func resolveSymbol&lt;ID>(id: ID) -> GraphicsContext.ResolvedSymbol?

Gets the identified child view as a resolved symbol, if the view exists.

struct ResolvedImage

An image resolved to a particular environment.

struct ResolvedText

A text view resolved to a particular environment.

