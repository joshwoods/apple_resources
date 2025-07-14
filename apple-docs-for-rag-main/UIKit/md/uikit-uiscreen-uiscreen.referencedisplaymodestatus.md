

- UIKit
- UIScreen
-  UIScreen.ReferenceDisplayModeStatus 

Enumeration

# UIScreen.ReferenceDisplayModeStatus

Describes a screen’s reference display mode status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+

``` source
enum ReferenceDisplayModeStatus
```

## Topics

### Statuses

case notSupported

A status that indicates the screen doesn’t provide a reference display mode.

case notEnabled

A status that indicates the screen provides a reference display mode but it’s in a disabled state.

case limited

A status that indicates the screen’s in a limited reference display mode.

case enabled

A status that indicates the screen’s in an accurate reference display mode.

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

### Getting the reference display mode status

var referenceDisplayModeStatus: UIScreen.ReferenceDisplayModeStatus

The status of the screen’s reference display mode.

var currentEDRHeadroom: CGFloat

The screen’s current headroom when displaying extended dynamic range content.

var potentialEDRHeadroom: CGFloat

The screen’s maximum headroom when displaying extended dynamic range content.

