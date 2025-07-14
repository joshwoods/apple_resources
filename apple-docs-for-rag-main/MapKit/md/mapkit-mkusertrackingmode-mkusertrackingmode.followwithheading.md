

- MapKit
- MKUserTrackingMode
-  MKUserTrackingMode.followWithHeading 

Case

# MKUserTrackingMode.followWithHeading

The map follows the user’s location and rotates when the heading changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+

``` source
case followWithHeading
```

## Discussion

This mode requires the device to have an available magnetometer. This mode isn’t available for compatible iPad or iPhone apps running in visionOS.

## See Also

### Constants

case none

The map doesn’t follow the user’s location.

case follow

The map follows the user location.

