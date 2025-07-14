

- AVFoundation
- AVCaption
-  textCombine(at:) 

Instance Method

# textCombine(at:)

Returns the text combine at the index position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func textCombine(at index: String.Index) -> (AVCaption.TextCombine, Range)
```

## Parameters 

`index`  

A character position in the caption text.

## Return Value

A tuple that contains the text combine color and range to which it applies.

## See Also

### Accessing Advanced Typography

func ruby(at: String.Index) -> (AVCaption.Ruby?, Range&lt;String.Index>)

Returns the ruby text at the index position.

class Ruby

An object that presents ruby characters.

enum TextCombine

The caption’s supported rendering policy options.

