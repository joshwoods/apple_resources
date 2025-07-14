

- HomeKit
-  HMCharacteristicTypeCurrentHorizontalTilt 

Global Variable

# HMCharacteristicTypeCurrentHorizontalTilt

The current tilt angle of a horizontal slat for an accessory like a window or a fan.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeCurrentHorizontalTilt: String
```

## Discussion

The corresponding value represents the angle in degrees, with a value between -90 and 90.

A value of -90 indicates the slats are fully closed and rotated such that the user-facing edge is higher than the opposing edge. A value of 0 indicates that the edges are at the same level, with the slats fully open.

## See Also

### Tilting mechanisms

let HMCharacteristicTypeTargetHorizontalTilt: String

The target tilt angle of a horizontal slat for an accessory like a window or a fan.

let HMCharacteristicTypeCurrentVerticalTilt: String

The current tilt angle of a vertical slat for an accessory like a window or a fan.

let HMCharacteristicTypeTargetVerticalTilt: String

The target tilt angle of a vertical slat for an accessory like a window or a fan.

let HMCharacteristicTypeCurrentTilt: String

The current tilt angle of a slat for an accessory like a window or a fan.

let HMCharacteristicTypeTargetTilt: String

The target tilt angle of a slat for an accessory like a window or a fan.

