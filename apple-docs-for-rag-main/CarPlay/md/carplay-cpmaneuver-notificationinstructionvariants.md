

- CarPlay
- CPManeuver
-  notificationInstructionVariants 

Instance Property

# notificationInstructionVariants

An array of instruction variants for notification banners.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var notificationInstructionVariants: [String] { get set }
```

## Discussion

Localize each variant for display to the user, and make sure the array contains at least one variant. The system displays the first variant that fits into the available screen space, so arrange the variants in order from most- to least-preferred.

Note

If you provide both notificationInstructionVariants and notificationAttributedInstructionVariants, the system displays instructions from the attributed instruction variants array. If you don’t provide notification variants, the system checks for attributedInstructionVariants, and then instructionVariants.

## See Also

### Providing instructions

var instructionVariants: [String]

An array of instruction variants for the maneuver.

var dashboardInstructionVariants: [String]

An array of instruction variants for the CarPlay dashboard.

