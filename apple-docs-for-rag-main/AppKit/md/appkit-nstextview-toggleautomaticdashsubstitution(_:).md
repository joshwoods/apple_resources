

- AppKit
- NSTextView
-  toggleAutomaticDashSubstitution(\_:) 

Instance Method

# toggleAutomaticDashSubstitution(\_:)

Toggles the state of the automatic dash substitution.

macOS 10.6+

``` source
@MainActor
func toggleAutomaticDashSubstitution(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message. May be `nil`.

## Discussion

Turning on automatic dash substitution enables automatic conversion of sequences of ASCII hyphen (`-`) characters to typographic dashes.

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

var isAutomaticDashSubstitutionEnabled: Bool

A Boolean value that indicates whether automatic dash substitution is enabled.

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

