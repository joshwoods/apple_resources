

- AVFoundation
- AVMutableCaption
-  setRuby(\_:in:) 

Instance Method

# setRuby(\_:in:)

Sets ruby text for a range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setRuby(
    _ rubyText: AVCaption.Ruby,
    in range: NSRange
)
```

## Parameters 

`rubyText`  

The ruby text.

`range`  

The range to which the ruby text applies.

## See Also

### Configuring Advanced Typography

class Ruby

An object that presents ruby characters.

func removeRuby(in: NSRange)

Removes ruby text from a range.

enum TextCombine

The caption’s supported rendering policy options.

func setTextCombine(AVCaption.TextCombine, in: NSRange)

Sets text combine for a range.

func removeTextCombine(in: NSRange)

Removes text combine from a range.

