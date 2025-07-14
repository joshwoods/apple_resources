

- SwiftUI
- Text
- Text.Layout
-  Text.Layout.RunSlice 

Structure

# Text.Layout.RunSlice

A slice of a run of placed glyphs in a text layout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct RunSlice
```

## Topics

### Initializers

init(run: Text.Layout.Run, indices: Range&lt;Int>)

### Instance Properties

var characterIndices: [Text.Layout.CharacterIndex]

The array of character indices corresponding to the glyphs in `self`.

var run: Text.Layout.Run

var typographicBounds: Text.Layout.TypographicBounds

The typographic bounds of the partial run of glyphs.

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

