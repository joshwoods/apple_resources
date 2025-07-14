

- CarPlay
-  CPManeuver 

Class

# CPManeuver

An object that describes a single navigation instruction.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPManeuver
```

## Overview

You use maneuvers to provide turn-by-turn guidance in navigation apps. Each maneuver represents a single navigation instruction and can include a symbol, an instruction, and estimates for remaining time and distance.

You supply an instruction as an array of variants, each with a different length. CarPlay chooses the longest variant that best fits the available space on the screen. You can optionally provide attributed variants that embed images using NSTextAttachment. See attributedInstructionVariants for more information.

In addition to the route guidance panel, you can show maneuvers on the CarPlay dashboard or in notification banners. Use the relevant properties to provide context-specific instructions and images.

## Topics

### Providing instructions

var instructionVariants: [String]

An array of instruction variants for the maneuver.

var dashboardInstructionVariants: [String]

An array of instruction variants for the CarPlay dashboard.

var notificationInstructionVariants: [String]

An array of instruction variants for notification banners.

### Providing attributed instructions

var attributedInstructionVariants: [NSAttributedString]

An array of attributed instruction variants for the maneuver.

var dashboardAttributedInstructionVariants: [NSAttributedString]

An array of attributed instruction variants for the CarPlay dashboard.

var notificationAttributedInstructionVariants: [NSAttributedString]

An array of attributed instruction variants for notification banners.

### Providing travel estimates

var initialTravelEstimates: CPTravelEstimates?

An object that describes the distance and time remaining before the maneuver completes.

### Providing symbol images

var symbolImage: UIImage?

An image that represents the maneuver.

var dashboardSymbolImage: UIImage?

An image for the CarPlay dashboard that represents the maneuver.

var notificationSymbolImage: UIImage?

An image for notification banners that represents the maneuver.

var symbolSet: CPImageSet?

An image set that represents the maneuver.

Deprecated

### Providing junction images

var junctionImage: UIImage?

An image that represents an upcoming junction.

var dashboardJunctionImage: UIImage?

An image for the CarPlay dashboard that represents an upcoming junction.

### Providing junction information

var junctionType: CPJunctionType

A value that represents the type of junction associated with this maneuver.

var junctionExitAngle: Measurement&lt;UnitAngle>?

The angle of the exit road of this junction.

var junctionElementAngles: Set&lt;Measurement&lt;UnitAngle>>?

A set of angles for the rest of the roads of this junction.

### Providing maneuver information

var maneuverType: CPManeuverType

A value that represents the type of maneuver.

var roadFollowingManeuverVariants: [String]?

An array of strings that represent the names of the road following this maneuver, arranged from most to least preferred.

var linkedLaneGuidance: CPLaneGuidance

A value that represents lane guidance associated with this maneuver.

var highwayExitLabel: String

A string that describes a highway exit.

var trafficSide: CPTrafficSide

A value that represents which side of the road the traffic drives on.

### Providing additional information

var userInfo: Any?

A custom object associated with the maneuver.

### Instance properties

var cardBackgroundColor: UIColor?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Maneuvers

enum CPManeuverState

Values that describe the state of a maneuver.

enum CPManeuverType

Values that describe types of navigation maneuvers.

