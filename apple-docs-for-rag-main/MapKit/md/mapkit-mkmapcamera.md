

- MapKit
-  MKMapCamera 

Class

# MKMapCamera

A virtual camera for defining the appearance of the map.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKMapCamera
```

## Overview

A camera object defines a virtual viewpoint above the map surface and affects how MapKit presents the map to the user. You use a camera object to specify the location of the camera on the map, the compass heading indicating the camera’s viewing direction, the pitch of the camera relative to the map perpendicular, and the camera’s altitude above the map. These factors create a map view with a three-dimensional perspective.

After creating an instance of this class, configure it with the desired attributes and assign it to your map view. When you assign a camera to your map view, MapKit centers the map using the value in your camera object’s centerCoordinate property, updating the map’s own region information in the process. The map also takes the camera’s pitch and altitude into account when calculating the visible region, ensuring that the region encompasses the visible content on the map.

## Topics

### Getting a camera object

convenience init(lookingAtCenter: CLLocationCoordinate2D, fromEyeCoordinate: CLLocationCoordinate2D, eyeAltitude: CLLocationDistance)

Returns a new camera object using the specified viewing angle information.

convenience init(lookingAtCenter: CLLocationCoordinate2D, fromDistance: CLLocationDistance, pitch: CGFloat, heading: CLLocationDirection)

Returns a new camera object using the specified distance, pitch, and heading information.

convenience init(lookingAt: MKMapItem, forViewSize: CGSize, allowPitch: Bool)

Returns a new camera object using the specified map item, view size, and pitch.

### Configuring the viewing angle

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

var heading: CLLocationDirection

The heading of the camera (in degrees) relative to true north.

var centerCoordinateDistance: CLLocationDistance

The distance from the center point of the map to the camera, in meters.

var pitch: CGFloat

The viewing angle of the camera, in degrees.

var altitude: CLLocationDistance

The altitude above the ground, in meters.

Deprecated

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

### Map customization

class MKCompassButton

A specialized view that displays the compass heading for its associated map.

class MKScaleView

A specialized view that displays the scale information for its associated map.

class MKZoomControl

A specialized view that displays and controls the zoom level of the map view.

class MKPitchControl

A specialized view that displays and controls the pitch angle of the map view.

class MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

class MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

