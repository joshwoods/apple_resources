

- UIKit
-  UITextAlternativeStyle 

Enumeration

# UITextAlternativeStyle

A constant that determines if the system highlights alternative phrases during text input.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UITextAlternativeStyle
```

## Topics

### Constants

case lowConfidence

A constant that indicates that the text input should highlight alternatives because the input text may be incorrect.

case none

A constant that indicates that the text input shouldn’t highlight alternatives because the input text is expected to be correct.

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

### Supporting text-phrase alternatives

func insertText(String, alternatives: [String], style: UITextAlternativeStyle)

