

- AVFoundation
- AVCaption
-  decoration(at:) 

Instance Method

# decoration(at:)

Returns the text decoration at the index position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func decoration(at index: String.Index) -> (AVCaption.Decoration, Range)
```

## Parameters 

`index`  

A character position in the caption text.

## Return Value

A tuple that contains the text decoration and range to which it applies.

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

struct Decoration

Text decorations for caption text.

