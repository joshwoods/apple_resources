

- UIKit
- UIScreen
-  referenceDisplayModeStatus 

Instance Property

# referenceDisplayModeStatus

The status of the screen’s reference display mode.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+

``` source
@MainActor
var referenceDisplayModeStatus: UIScreen.ReferenceDisplayModeStatus { get }
```

## Discussion

Note

*Reference display mode* refers to Pro Display Mode on the iPad Pro 12.9-inch (5th generation or later).

## See Also

### Getting the reference display mode status

enum ReferenceDisplayModeStatus

Describes a screen’s reference display mode status.

var currentEDRHeadroom: CGFloat

The screen’s current headroom when displaying extended dynamic range content.

var potentialEDRHeadroom: CGFloat

The screen’s maximum headroom when displaying extended dynamic range content.

