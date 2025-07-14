

- UIKit
-  UITextInlinePredictionType 

Enumeration

# UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
enum UITextInlinePredictionType
```

## Overview

Use these constants with the inlinePredictionType property.

## Topics

### Constants

case `default`

A constant that determines the behavior of inline text predictions according to the context.

case no

A constant that turns off inline text predictions.

case yes

A constant that turns on inline text predictions.

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

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

