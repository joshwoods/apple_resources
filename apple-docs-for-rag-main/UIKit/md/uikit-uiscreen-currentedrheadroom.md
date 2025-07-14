

- UIKit
- UIScreen
-  currentEDRHeadroom 

Instance Property

# currentEDRHeadroom

The screen’s current headroom when displaying extended dynamic range content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+

``` source
@MainActor
var currentEDRHeadroom: CGFloat { get }
```

## Discussion

*Headroom* is the ratio of the luminance of the screen’s brightest white to the luminance of standard dynamic range (SDR) white, in the screen’s native color space. The screen’s current headroom limits all rendered content, and can change depending on its configuration and whether it’s displaying extended dynamic range (EDR) content.

To display EDR content in a CAMetalLayer, set the layer’s wantsExtendedDynamicRangeContent property to true.

## See Also

### Getting the reference display mode status

var referenceDisplayModeStatus: UIScreen.ReferenceDisplayModeStatus

The status of the screen’s reference display mode.

enum ReferenceDisplayModeStatus

Describes a screen’s reference display mode status.

var potentialEDRHeadroom: CGFloat

The screen’s maximum headroom when displaying extended dynamic range content.

