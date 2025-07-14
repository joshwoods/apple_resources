

- UIKit
-  UITextAutocorrectionType 

Enumeration

# UITextAutocorrectionType

The autocorrection behavior of a text-based view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UITextAutocorrectionType
```

## Overview

Use these constants with the autocorrectionType property. If the script system doesn’t support inline autocorrection, the keyboard input method ignores these constants.

## Topics

### Constants

case `default`

Specifies an appropriate autocorrection behavior for the current script system.

case no

Disables autocorrection behavior.

case yes

Enables autocorrection behavior.

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

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

var autocorrectionType: UITextAutocorrectionType

The autocorrection style for the text object.

var spellCheckingType: UITextSpellCheckingType

The spell-checking style for the text object.

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

