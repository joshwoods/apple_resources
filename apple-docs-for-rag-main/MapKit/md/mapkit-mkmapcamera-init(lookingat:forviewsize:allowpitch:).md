

- MapKit
- MKMapCamera
-  init(lookingAt:forViewSize:allowPitch:) 

Initializer

# init(lookingAt:forViewSize:allowPitch:)

Returns a new camera object using the specified map item, view size, and pitch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
convenience init(
    lookingAt mapItem: MKMapItem,
    forViewSize viewSize: CGSize,
    allowPitch: Bool
)
```

## Parameters 

`mapItem`  

An MKMapItem that indicates the location of the camera.

`viewSize`  

The view’s size.

`allowPitch`  

A Boolean value that indicates if the camera should the use map’s pitch angle.

## See Also

### Getting a camera object

convenience init(lookingAtCenter: CLLocationCoordinate2D, fromEyeCoordinate: CLLocationCoordinate2D, eyeAltitude: CLLocationDistance)

Returns a new camera object using the specified viewing angle information.

convenience init(lookingAtCenter: CLLocationCoordinate2D, fromDistance: CLLocationDistance, pitch: CGFloat, heading: CLLocationDirection)

Returns a new camera object using the specified distance, pitch, and heading information.

