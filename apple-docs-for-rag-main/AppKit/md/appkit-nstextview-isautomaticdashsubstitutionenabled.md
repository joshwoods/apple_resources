

- AppKit
- NSTextView
-  isAutomaticDashSubstitutionEnabled 

Instance Property

# isAutomaticDashSubstitutionEnabled

A Boolean value that indicates whether automatic dash substitution is enabled.

macOS 10.6+

``` source
@MainActor
var isAutomaticDashSubstitutionEnabled: Bool { get set }
```

## Discussion

true if it is enabled, otherwise false.

Turning on automatic dash substitution enables automatic conversion of a two ASCII hyphen (`-`) characters into an em-dash.

## See Also

### Checking and substituting text

func checkTextInDocument(Any?)

Performs the default text checking on the entire document.

func checkTextInSelection(Any?)

Performs the default text checking on the current selection.

func checkText(in: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any])

Check and replace the text in the range using the specified checking types and options.

func handleTextCheckingResults([NSTextCheckingResult], forRange: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any], orthography: NSOrthography, wordCount: Int)

Handles the text checking results returned by the text view

var enabledTextCheckingTypes: NSTextCheckingTypes

The default text checking types.

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

