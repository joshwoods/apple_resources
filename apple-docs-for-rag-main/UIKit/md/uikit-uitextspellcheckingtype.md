

- UIKit
-  UITextSpellCheckingType 

Enumeration

# UITextSpellCheckingType

The spell-checking behavior of a text-based view.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum UITextSpellCheckingType
```

## Overview

Use these constants with the spellCheckingType property.

## Topics

### Constants

case `default`

Specifies the default spell-checking behavior.

case no

Disables spell-checking behavior.

case yes

Enables spell-checking behavior.

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

enum UITextAutocorrectionType

The autocorrection behavior of a text-based view.

var spellCheckingType: UITextSpellCheckingType

The spell-checking style for the text object.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

