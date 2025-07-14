

- MapKit
- MKMapCamera
-  init(lookingAtCenter:fromEyeCoordinate:eyeAltitude:) 

Initializer

# init(lookingAtCenter:fromEyeCoordinate:eyeAltitude:)

Returns a new camera object using the specified viewing angle information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    lookingAtCenter centerCoordinate: CLLocationCoordinate2D,
    fromEyeCoordinate eyeCoordinate: CLLocationCoordinate2D,
    eyeAltitude: CLLocationDistance
)
```

## Parameters 

`centerCoordinate`  

The coordinate point on which the framework centers the map.

`eyeCoordinate`  

The coordinate point at which to place the camera. If the value for this parameter is equal to the value in the `centerCoordinate` parameter, the framework displays the map as if the camera is looking straight down. If this point is offset from the `centerCoordinate` value, the framework displays the map with an appropriate heading and pitch angle.

`eyeAltitude`  

The altitude (in meters) above the ground at which to place the camera.

## Return Value

A new camera object that initializes with the specified information.

## Discussion

This method calculates the required pitch and heading angles to accommodate the specified eye position and altitude.

## See Also

### Getting a camera object

convenience init(lookingAtCenter: CLLocationCoordinate2D, fromDistance: CLLocationDistance, pitch: CGFloat, heading: CLLocationDirection)

Returns a new camera object using the specified distance, pitch, and heading information.

convenience init(lookingAt: MKMapItem, forViewSize: CGSize, allowPitch: Bool)

Returns a new camera object using the specified map item, view size, and pitch.

