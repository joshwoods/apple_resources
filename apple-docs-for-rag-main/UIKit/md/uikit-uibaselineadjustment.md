

- UIKit
-  UIBaselineAdjustment 

Enumeration

# UIBaselineAdjustment

Vertical adjustment options.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIBaselineAdjustment
```

## Overview

Baseline adjustment options determine how to adjust the position of text in cases where the text must be drawn using a different font size than the one originally specified. For example, with the UIBaselineAdjustment.alignBaselines option, the position of the baseline remains fixed at its initial location while the text appears to move toward that baseline. Similarly, the UIBaselineAdjustment.none option makes it appear as if the text is moving upwards toward the top-left corner of the bounding box.

## Topics

### Constants

case alignBaselines

Adjust text relative to the position of its baseline.

case alignCenters

Adjust text relative to the center of its bounding box.

case none

Adjust text relative to the top-left corner of the bounding box.

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

### Strings

class NSStringDrawingContext

An object that manages metrics for drawing attributed strings.

struct NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

