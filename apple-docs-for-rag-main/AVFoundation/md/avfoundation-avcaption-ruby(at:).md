

- AVFoundation
- AVCaption
-  ruby(at:) 

Instance Method

# ruby(at:)

Returns the ruby text at the index position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func ruby(at index: String.Index) -> (AVCaption.Ruby?, Range)
```

## Parameters 

`index`  

A character position in the caption text.

## Return Value

A tuple that contains the ruby text and range to which it applies.

## See Also

### Accessing Advanced Typography

class Ruby

An object that presents ruby characters.

func textCombine(at: String.Index) -> (AVCaption.TextCombine, Range&lt;String.Index>)

Returns the text combine at the index position.

enum TextCombine

The caption’s supported rendering policy options.

