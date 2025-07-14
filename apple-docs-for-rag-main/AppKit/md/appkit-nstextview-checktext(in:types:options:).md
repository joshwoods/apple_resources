

- AppKit
- NSTextView
-  checkText(in:types:options:) 

Instance Method

# checkText(in:types:options:)

Check and replace the text in the range using the specified checking types and options.

macOS 10.6+

``` source
@MainActor
func checkText(
    in range: NSRange,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any] = [:]
)
```

## Parameters 

`range`  

The range to check.

`checkingTypes`  

The type of checking to be performed, passed by-reference. The possible constants are listed in NSTextCheckingTypes and can be combined using the C bit-wise `OR` operator to perform multiple checks at the same time.

`options`  

A dictionary of values used during the checking process to perform. See Spell Checking Option Dictionary Keys for the supported values.

## Discussion

This method calls the delegate method textView(_:willCheckTextIn:options:types:) allowing you to modify the parameters before the checking occurs.

This method usually would not be called directly, since `NSTextView` itself will call it as needed, but it can be overridden.

## See Also

### Checking and substituting text

func checkTextInDocument(Any?)

Performs the default text checking on the entire document.

func checkTextInSelection(Any?)

Performs the default text checking on the current selection.

func handleTextCheckingResults([NSTextCheckingResult], forRange: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any], orthography: NSOrthography, wordCount: Int)

Handles the text checking results returned by the text view

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

