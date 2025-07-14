

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.State
-  ARGeoTrackingStatus.State.localizing 

Case

# ARGeoTrackingStatus.State.localizing

Geo tracking is attempting to localize against a map.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case localizing
```

## Discussion

In ARGeoTrackingStatus.State.localizing, the session downloads localization imagery for the user’s geographic location and compares it with captures from the device’s camera. This process is referred to as *visual localization*. When ARKit succeeds in matching this imagery with captures from the camera, the state moves to ARGeoTrackingStatus.State.localized and the app is free to create location anchors. For more information about localization imagery, see Refine the User’s Position with Imagery.

### Assisting the User with Visual Localization

To establish visual localization, the user must move the camera so it acquires the captures that ARKit needs. To elicit the right user movements in ARGeoTrackingStatus.State.localizing, the app needs to advise the user to:

- Point the camera at buildings and other visual landmarks to help ARKit match the live camera data with its preexisting landscape-data.

- Avoid pointing the device at objects that are too general, like trees. It’s better to focus on distinct visuals, like structures, or signs.

- Avoid pointing the device at real-world objects that are transient, like parked cars, or a construction site.

- Because lighting conditions can affect visual localization, avoid geo tracking at night.

## See Also

### States

case initializing

The session is initializing geo tracking.

case localized

Geo tracking is localized.

case notAvailable

Geo tracking is not available.

case initializing

The session is initializing geo tracking.

case localized

Geo tracking is localized.

case notAvailable

Geo tracking is not available.

