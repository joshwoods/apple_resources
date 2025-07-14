

- SwiftUI
- Text
-  Text.Layout 

Structure

# Text.Layout

A value describing the layout and custom attributes of a tree of `Text` views.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Layout
```

## Topics

### Structures

struct CharacterIndex

The index of a character in the source text. An opaque type, this is intended to be used to determine relative locations of elements in the layout, rather than how they map to the source strings.

struct DrawingOptions

Option flags used when drawing `Text.Layout` lines or runs into a graphics context.

struct Line

A single line in a text layout: a collection of runs of placed glyphs.

struct Run

A run of placed glyphs in a text layout.

struct RunSlice

A slice of a run of placed glyphs in a text layout.

struct TypographicBounds

The typographic bounds of an element in a text layout.

### Instance Properties

var isTruncated: Bool

Indicates if this text is truncated.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- RandomAccessCollection
- Sequence

