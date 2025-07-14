

- CarPlay
- CPManeuver
-  instructionVariants 

Instance Property

# instructionVariants

An array of instruction variants for the maneuver.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var instructionVariants: [String] { get set }
```

## Discussion

Localize each variant for display to the user, and make sure the array contains at least one variant. The system displays the first variant that fits into the available screen space, so arrange the variants in order from most- to least-preferred.

Note

If you provide both instructionVariants and attributedInstructionVariants, the system displays instructions from the attributed instruction variants array.

## See Also

### Providing instructions

var dashboardInstructionVariants: [String]

An array of instruction variants for the CarPlay dashboard.

var notificationInstructionVariants: [String]

An array of instruction variants for notification banners.

