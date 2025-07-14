

- AVFoundation
- AVCaption
-  fontWeight(at:) 

Instance Method

# fontWeight(at:)

Returns the font weight and range at the index position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func fontWeight(at index: String.Index) -> (AVCaption.FontWeight, Range)
```

## Parameters 

`index`  

A character position in the caption text.

## Return Value

A tuple that contains the font weight and range to which it applies.

## See Also

### Accessing Font Styles

func fontStyle(at: String.Index) -> (AVCaption.FontStyle, Range&lt;String.Index>)

Returns the font style and range at the index position.

enum FontStyle

Font styles for caption text.

enum FontWeight

Font weights for a caption.

func decoration(at: String.Index) -> (AVCaption.Decoration, Range&lt;String.Index>)

Returns the text decoration at the index position.

struct Decoration

Text decorations for caption text.

