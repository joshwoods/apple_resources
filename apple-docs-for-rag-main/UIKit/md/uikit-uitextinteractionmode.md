

- UIKit
-  UITextInteractionMode 

Enumeration

# UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UITextInteractionMode
```

## Topics

### Modes

case editable

A mode indicating that the text interaction should provide selection behaviors for editable text.

case nonEditable

A mode indicating that the text interaction should provide selection behaviors for non-editable, read-only text.

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

### Text interactions

class UITextInteraction

An interaction that provides text selection gestures and UI to custom text views.

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

