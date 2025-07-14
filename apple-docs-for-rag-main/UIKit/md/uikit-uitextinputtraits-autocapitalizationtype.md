

- UIKit
- UITextInputTraits
-  autocapitalizationType 

Instance Property

# autocapitalizationType

The autocapitalization style for the text object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var autocapitalizationType: UITextAutocapitalizationType { get set }
```

## Discussion

This property determines at what times the Shift key is automatically pressed, thereby making the typed character a capital letter. The default value for this property is UITextAutocapitalizationType.sentences.

Some keyboard types do not support autocapitalization. Specifically, this option is ignored if the value in the keyboardType property is set to UIKeyboardType.numberPad, UIKeyboardType.phonePad, or UIKeyboardType.namePhonePad.

## See Also

### Managing spelling and autocorrection

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

var autocorrectionType: UITextAutocorrectionType

The autocorrection style for the text object.

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

