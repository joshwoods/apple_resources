

- UIKit
- UITextInputTraits
-  autocorrectionType 

Instance Property

# autocorrectionType

The autocorrection style for the text object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var autocorrectionType: UITextAutocorrectionType { get set }
```

## Discussion

This property determines whether autocorrection is enabled or disabled during typing. With autocorrection enabled, the text object tracks unknown words and suggests a more suitable replacement candidate to the user, replacing the typed text automatically unless the user explicitly overrides the action.

The default value for this property is UITextAutocorrectionType.default, which for most input methods results in autocorrection being enabled.

## See Also

### Managing spelling and autocorrection

var autocapitalizationType: UITextAutocapitalizationType

The autocapitalization style for the text object.

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

enum UITextAutocorrectionType

The autocorrection behavior of a text-based view.

var spellCheckingType: UITextSpellCheckingType

The spell-checking style for the text object.

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

