

- ARKit
- ARConfiguration
- ARConfiguration.WorldAlignment
-  ARConfiguration.WorldAlignment.gravityAndHeading 

Case

# ARConfiguration.WorldAlignment.gravityAndHeading

The coordinate system’s y-axis is parallel to gravity, its x- and z-axes are oriented to compass heading, and its origin is the initial position of the device.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case gravityAndHeading
```

## Discussion

The y-axis matches the direction of gravity as detected by the device’s motion sensing hardware; that is, the vector `(0,-1,0)` points downward.

The x- and z-axes match the longitude and latitude directions as measured by Location Services. The vector `(0,0,-1)` points to true north and the vector `(-1,0,0)` points west. (That is, the positive x-, y-, and z-axes point east, up, and south, respectively.)

Although this option fixes the *directions* of the three coordinate axes to real-world directions, the *location* of the coordinate system’s origin is still relative to the device, matching the device’s position as of when the session configuration is first run.

Note

Using gravity and heading alignment requires tracking the device’s geographic location. Your app’s Info.plist must include user-facing text for the NSLocationUsageDescription or NSLocationWhenInUseUsageDescription key so that the user can grant your app permission for location tracking.

## See Also

### Alignments

case gravity

The coordinate system’s y-axis is parallel to gravity, and its origin is the initial position of the device.

case camera

The scene coordinate system is locked to match the orientation of the camera.

