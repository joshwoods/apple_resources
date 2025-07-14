

- AppKit
- NSTextViewDelegate
-  textView(\_:didCheckTextIn:types:options:results:orthography:wordCount:) 

Instance Method

# textView(\_:didCheckTextIn:types:options:results:orthography:wordCount:)

Invoked to allow the delegate to modify the text checking results after checking has occurred.

macOS 10.6+

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    didCheckTextIn range: NSRange,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any] = [:],
    results: [NSTextCheckingResult],
    orthography: NSOrthography,
    wordCount: Int
) -> [NSTextCheckingResult]
```

## Parameters 

`view`  

The text view sending the message.

`range`  

The range that was checked.

`checkingTypes`  

The type of checking that was performed. The possible constants are listed in NSTextCheckingTypes and can be combined using the C bit-wise `OR` operator to perform multiple checks at the same time.

`options`  

A dictionary of values used during the checking process to perform. See Spell Checking Option Dictionary Keys for the supported values.

`results`  

An array of NSTextCheckingResult instances.

`orthography`  

The orthography of the text.

`wordCount`  

The number of words checked.

## Return Value

An array of NSTextCheckingResult instances. You can return the results array as is, or an altered array of NSTextCheckingResult objects.

## Discussion

Invoked by handleTextCheckingResults(_:forRange:types:options:orthography:wordCount:), this method allows observation of text checking, or modification of the results

## See Also

### Working With the Spelling Checker

func textView(NSTextView, shouldSetSpellingState: Int, range: NSRange) -> Int

Sent when the spelling state is changed.

func textView(NSTextView, willCheckTextIn: NSRange, options: [NSSpellChecker.OptionKey : Any], types: UnsafeMutablePointer&lt;NSTextCheckingTypes>) -> [NSSpellChecker.OptionKey : Any]

Invoked to allow the delegate to modify the text checking process before it occurs.

