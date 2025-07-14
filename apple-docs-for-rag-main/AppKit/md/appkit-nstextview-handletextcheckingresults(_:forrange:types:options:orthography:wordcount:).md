

- AppKit
- NSTextView
-  handleTextCheckingResults(\_:forRange:types:options:orthography:wordCount:) 

Instance Method

# handleTextCheckingResults(\_:forRange:types:options:orthography:wordCount:)

Handles the text checking results returned by the text view

macOS 10.6+

``` source
@MainActor
func handleTextCheckingResults(
    _ results: [NSTextCheckingResult],
    forRange range: NSRange,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any] = [:],
    orthography: NSOrthography,
    wordCount: Int
)
```

## Parameters 

`results`  

An array of NSTextCheckingResult objects.

`range`  

The range of text that was checked.

`checkingTypes`  

The type of checking performed. The possible constants are listed in NSTextCheckingTypes and can be combined using the C bit-wise `OR` operator to perform multiple checks at the same time.

`options`  

The dictionary of values used during the checking process to perform. See Spell Checking Option Dictionary Keys for the supported values.

`orthography`  

The orthography of the checked text.

`wordCount`  

The number of words.

## Discussion

The NSTextViewDelegate offers a method, textView(_:didCheckTextIn:types:options:results:orthography:wordCount:) that is called after the checking is performed, allowing you to modify the results.

This method usually would not be called directly, since `NSTextView` itself will call it as needed, but it can be overridden.

## See Also

### Checking and substituting text

func checkTextInDocument(Any?)

Performs the default text checking on the entire document.

func checkTextInSelection(Any?)

Performs the default text checking on the current selection.

func checkText(in: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any])

Check and replace the text in the range using the specified checking types and options.

var enabledTextCheckingTypes: NSTextCheckingTypes

The default text checking types.

var isAutomaticDashSubstitutionEnabled: Bool

A Boolean value that indicates whether automatic dash substitution is enabled.

func toggleAutomaticDashSubstitution(Any?)

Toggles the state of the automatic dash substitution.

var isAutomaticDataDetectionEnabled: Bool

A Boolean value that indicates whether automatic data detection is enabled.

func toggleAutomaticDataDetection(Any?)

Toggles the state of the automatic data detection.

var isAutomaticSpellingCorrectionEnabled: Bool

A Boolean value that indicates whether automatic spelling correction is enabled.

func toggleAutomaticSpellingCorrection(Any?)

Toggles the state of the automatic spelling correction.

var isAutomaticTextReplacementEnabled: Bool

A Boolean value that indicates whether automatic text replacement is enabled.

func toggleAutomaticTextReplacement(Any?)

Toggles the state of the automatic text replacement.

func performValidatedReplacement(in: NSRange, with: NSAttributedString) -> Bool

Replaces text in the range you specify with the attributed string you provide.

