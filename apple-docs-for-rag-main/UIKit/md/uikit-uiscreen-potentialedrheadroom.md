

- UIKit
- UIScreen
-  potentialEDRHeadroom 

Instance Property

# potentialEDRHeadroom

The screen’s maximum headroom when displaying extended dynamic range content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+

``` source
@MainActor
var potentialEDRHeadroom: CGFloat { get }
```

## Discussion

*Headroom* is the ratio of the luminance of the screen’s brightest white to the luminance of standard dynamic range (SDR) white, in the screen’s native color space. The screen’s maximum headroom can change depending on its configuration, such as when referenceDisplayModeStatus changes.

You can query this property even when the screen isn’t displaying extended dynamic range (EDR) content.

## See Also

### Getting the reference display mode status

var referenceDisplayModeStatus: UIScreen.ReferenceDisplayModeStatus

The status of the screen’s reference display mode.

enum ReferenceDisplayModeStatus

Describes a screen’s reference display mode status.

var currentEDRHeadroom: CGFloat

The screen’s current headroom when displaying extended dynamic range content.

