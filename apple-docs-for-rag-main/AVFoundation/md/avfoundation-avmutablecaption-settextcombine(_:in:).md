

- AVFoundation
- AVMutableCaption
-  setTextCombine(\_:in:) 

Instance Method

# setTextCombine(\_:in:)

Sets text combine for a range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setTextCombine(
    _ textCombine: AVCaption.TextCombine,
    in range: NSRange
)
```

## Parameters 

`textCombine`  

The text combine.

`range`  

The range to which the text combine applies.

## See Also

### Configuring Advanced Typography

class Ruby

An object that presents ruby characters.

func setRuby(AVCaption.Ruby, in: NSRange)

Sets ruby text for a range.

func removeRuby(in: NSRange)

Removes ruby text from a range.

enum TextCombine

The caption’s supported rendering policy options.

func removeTextCombine(in: NSRange)

Removes text combine from a range.

