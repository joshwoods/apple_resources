

- AVFoundation
- AVCaption
-  AVCaption.Decoration 

Structure

# AVCaption.Decoration

Text decorations for caption text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Decoration
```

## Topics

### Decorations

static var underline: AVCaption.Decoration

A decoration representing a line under the text.

static var lineThrough: AVCaption.Decoration

A decoration representing a line through the text.

static var overline: AVCaption.Decoration

A decoration representing a line over the text.

### Initializers

init(rawValue: UInt)

Creates a caption decoration by using a string.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing Font Styles

func fontStyle(at: String.Index) -> (AVCaption.FontStyle, Range&lt;String.Index>)

Returns the font style and range at the index position.

enum FontStyle

Font styles for caption text.

func fontWeight(at: String.Index) -> (AVCaption.FontWeight, Range&lt;String.Index>)

Returns the font weight and range at the index position.

enum FontWeight

Font weights for a caption.

func decoration(at: String.Index) -> (AVCaption.Decoration, Range&lt;String.Index>)

Returns the text decoration at the index position.

