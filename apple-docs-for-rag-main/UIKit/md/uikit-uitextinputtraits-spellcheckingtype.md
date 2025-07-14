

- UIKit
- UITextInputTraits
-  spellCheckingType 

Instance Property

# spellCheckingType

The spell-checking style for the text object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional var spellCheckingType: UITextSpellCheckingType { get set }
```

## Discussion

This property determines whether spell-checking is enabled or disabled during typing. With spell-checking enabled, the text object generates red underlines for all misspelled words. If the user taps on a misspelled word, the text object presents the user with a list of possible corrections.

The default value for this property is UITextSpellCheckingType.default, which enables spell-checking when autocorrection is also enabled. The value in this property overrides the spell-checking setting set by the user in Settings \> General \> Keyboard.

## See Also

### Managing spelling and autocorrection

var autocapitalizationType: UITextAutocapitalizationType

The autocapitalization style for the text object.

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

var autocorrectionType: UITextAutocorrectionType

The autocorrection style for the text object.

enum UITextAutocorrectionType

The autocorrection behavior of a text-based view.

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

