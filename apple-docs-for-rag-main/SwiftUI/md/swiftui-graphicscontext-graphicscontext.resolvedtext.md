

- SwiftUI
- GraphicsContext
-  GraphicsContext.ResolvedText 

Structure

# GraphicsContext.ResolvedText

A text view resolved to a particular environment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ResolvedText
```

## Overview

You resolve a Text view in preparation for drawing it into a context, either manually by calling resolve(_:) or automatically when calling draw(_:in:) or draw(_:at:anchor:). The resolved text view takes into account environment values like the display resolution and current color scheme.

## Topics

### Getting the text properties

func firstBaseline(in: CGSize) -> CGFloat

Gets the distance from the first line’s ascender to its baseline.

func lastBaseline(in: CGSize) -> CGFloat

Gets the distance from the first line’s ascender to the last line’s baseline.

func measure(in: CGSize) -> CGSize

Measures the size of the resolved text for a given area into which the text should be placed.

var shading: GraphicsContext.Shading

The shading to fill uncolored text regions with.

## See Also

### Resolving a drawn entity

func resolve(_:)

Gets a version of an image that’s fixed with the current values of the graphics context’s environment.

func resolveSymbol&lt;ID>(id: ID) -> GraphicsContext.ResolvedSymbol?

Gets the identified child view as a resolved symbol, if the view exists.

struct ResolvedSymbol

A static sequence of drawing operations that may be drawn multiple times, preserving their resolution independence.

struct ResolvedImage

An image resolved to a particular environment.

