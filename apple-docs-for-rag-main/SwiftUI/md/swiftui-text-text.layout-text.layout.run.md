

- SwiftUI
- Text
- Text.Layout
-  Text.Layout.Run 

Structure

# Text.Layout.Run

A run of placed glyphs in a text layout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Run
```

## Topics

### Instance Properties

var characterIndices: [Text.Layout.CharacterIndex]

The array of character indices corresponding to the glyphs in `self`.

var layoutDirection: LayoutDirection

The layout direction of the text run.

var typographicBounds: Text.Layout.TypographicBounds

The typographic bounds of the run of glyphs.

### Subscripts

subscript&lt;T>(T.Type) -> T?

The custom attribute of type `T` associated with the run of glyphs, or nil.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- RandomAccessCollection
- Sequence

