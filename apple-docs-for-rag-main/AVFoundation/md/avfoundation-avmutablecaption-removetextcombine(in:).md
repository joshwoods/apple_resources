

- AVFoundation
- AVMutableCaption
-  removeTextCombine(in:) 

Instance Method

# removeTextCombine(in:)

Removes text combine from a range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func removeTextCombine(in range: NSRange)
```

## Parameters 

`range`  

The range from which the system removes text combine.

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

func setTextCombine(AVCaption.TextCombine, in: NSRange)

Sets text combine for a range.

