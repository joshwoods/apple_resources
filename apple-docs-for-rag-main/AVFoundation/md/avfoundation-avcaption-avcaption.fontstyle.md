

- AVFoundation
- AVCaption
-  AVCaption.FontStyle 

Enumeration

# AVCaption.FontStyle

Font styles for caption text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum FontStyle
```

## Topics

### Font Styles

case unknown

An unknown font style.

case normal

A normal font style.

case italic

An italic font style.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Font Styles

func fontStyle(at: String.Index) -> (AVCaption.FontStyle, Range&lt;String.Index>)

Returns the font style and range at the index position.

func fontWeight(at: String.Index) -> (AVCaption.FontWeight, Range&lt;String.Index>)

Returns the font weight and range at the index position.

enum FontWeight

Font weights for a caption.

func decoration(at: String.Index) -> (AVCaption.Decoration, Range&lt;String.Index>)

Returns the text decoration at the index position.

struct Decoration

Text decorations for caption text.

