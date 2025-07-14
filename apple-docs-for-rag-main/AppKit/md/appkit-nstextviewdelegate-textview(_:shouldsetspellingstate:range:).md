

- AppKit
- NSTextViewDelegate
-  textView(\_:shouldSetSpellingState:range:) 

Instance Method

# textView(\_:shouldSetSpellingState:range:)

Sent when the spelling state is changed.

macOS 10.5+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    shouldSetSpellingState value: Int,
    range affectedCharRange: NSRange
) -> Int
```

## Parameters 

`textView`  

The text view sending the message.

`value`  

The proposed spelling state value to set. Possible values, for the temporary attribute on the layout manager using the key NSSpellingStateAttributeName, are:

- NSSpellingStateSpellingFlag to highlight spelling issues.

- NSSpellingStateGrammarFlag to highlight grammar issues.

`affectedCharRange`  

The character range over which to set the given spelling state.

## Return Value

The actual spelling state to set.

## Discussion

Delegate only. Allows delegate to control the setting of spelling and grammar indicators.

## See Also

### Related Documentation

func setSpellingState(Int, range: NSRange)

Sets the spelling state, which controls the display of the spelling and grammar indicators on the given text range.

### Working With the Spelling Checker

func textView(NSTextView, willCheckTextIn: NSRange, options: [NSSpellChecker.OptionKey : Any], types: UnsafeMutablePointer&lt;NSTextCheckingTypes>) -> [NSSpellChecker.OptionKey : Any]

Invoked to allow the delegate to modify the text checking process before it occurs.

func textView(NSTextView, didCheckTextIn: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any], results: [NSTextCheckingResult], orthography: NSOrthography, wordCount: Int) -> [NSTextCheckingResult]

Invoked to allow the delegate to modify the text checking results after checking has occurred.

