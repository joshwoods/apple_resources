

- AppKit
- NSTextViewDelegate
-  textView(\_:willCheckTextIn:options:types:) 

Instance Method

# textView(\_:willCheckTextIn:options:types:)

Invoked to allow the delegate to modify the text checking process before it occurs.

macOS 10.6+

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    willCheckTextIn range: NSRange,
    options: [NSSpellChecker.OptionKey : Any] = [:],
    types checkingTypes: UnsafeMutablePointer
) -> [NSSpellChecker.OptionKey : Any]
```

## Parameters 

`view`  

The text view sending the message.

`range`  

The range to be checked.

`options`  

A dictionary of values used during the checking process to perform. See Spell Checking Option Dictionary Keys for the supported values.

`checkingTypes`  

The type of checking to be performed, passed by-reference. The possible constants are listed in NSTextCheckingTypes and can be combined using the C bit-wise `OR` operator to perform multiple checks at the same time.

You can change this parameter to alter the types of checking to be performed.

## Return Value

A dictionary containing an alternative to the options `dictionary`.

## Discussion

Invoked by checkText(in:types:options:), this method allows control over text checking `options`s (via the return value) or types (by modifying the flags pointed to by the inout parameter `checkingTypes`)

## See Also

### Working With the Spelling Checker

func textView(NSTextView, shouldSetSpellingState: Int, range: NSRange) -> Int

Sent when the spelling state is changed.

func textView(NSTextView, didCheckTextIn: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any], results: [NSTextCheckingResult], orthography: NSOrthography, wordCount: Int) -> [NSTextCheckingResult]

Invoked to allow the delegate to modify the text checking results after checking has occurred.

