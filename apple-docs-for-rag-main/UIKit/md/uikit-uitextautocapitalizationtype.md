

- UIKit
-  UITextAutocapitalizationType 

Enumeration

# UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UITextAutocapitalizationType
```

## Overview

Use these constants with the autocapitalizationType property. If the script system doesn’t support capitalization, the keyboard input method ignores these constants.

Some keyboard types don’t support autocapitalization. Specifically, if the keyboardType property is set to UIKeyboardType.numberPad, UIKeyboardType.phonePad, or UIKeyboardType.namePhonePad, the system ignores these constants.

## Topics

### Constants

case none

Specifies that there is no automatic text capitalization.

case words

Specifies automatic capitalization of the first letter of each word.

case sentences

Specifies automatic capitalization of the first letter of each sentence.

case allCharacters

Specifies automatic capitalization of all characters, such as for entry of two-character state abbreviations for the United States.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing spelling and autocorrection

var autocapitalizationType: UITextAutocapitalizationType

The autocapitalization style for the text object.

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

