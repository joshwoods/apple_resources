

- ARKit
-  ARGeoAnchor 

Class

# ARGeoAnchor

An anchor that identifies a geographic location using latitude, longitude, and altitude data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ARGeoAnchor
```

## Overview

A *geographic anchor* (also known as *location anchor*) identifies a specific area in the world that the app can refer to in an AR experience. As a user moves around the scene, the session updates a location anchor’s transform based on the anchor’s coordinate and the device’s compass heading.

ARKit aligns location anchors to an East-North-Up orientation, with its x- and z-axes matching the longitude and latitude directions. For more information, see ARConfiguration.WorldAlignment.gravityAndHeading.

ARKit sets the anchor’s vertical position to the altitude you pass in to initWithCoordinate:altitude:. If you initialize a location anchor using initWithCoordinate: instead, ARKit sets the anchor’s altitude to ground level.

Important

Location anchors are available only in geotracking sessions, and geotracking is available in specific areas; for more information, see ARGeoTrackingConfiguration.

### Communicate Data Usage

Location anchors consume data from Apple Maps called *localization imagery* (for more information, see ARGeoTrackingConfiguration). As the user moves, the framework downloads localization imagery to refine the user’s precise geographic position. The amount of data the session requires depends on the user’s movement and distance they travel. To make the user aware of potential fees, you can notify the user of their data usage.

### Manage Location Anchor Availability

When an app creates a location anchor, it’s invisible to the user until the framework *populates* the anchor in the scene. When an anchor populates successfully, the session passes the anchor into the delegate’s session(_:didAdd:) callback.

If ARKit fails to populate a location anchor, the session calls session(_:didRemove:) to notify your delegate. A location anchor may fail to populate when:

- The network is unavailable. If you create a location anchor without providing an altitude, ARKit defaults the altitude to ground level, and may query the server to check the topography at the anchor’s geographic coordinate. If the network is unavailable, ask the user to restore a connection by disabling Airplane Mode, enabling WiFi, or moving to a location that provides service. If the network is available but slow, an altitude query response may be delayed. Consider pausing a navigation or presenting visual feedback for the anchor’s tentative placement, such as by displaying a status indicator.

- The location anchor is too far from the user. If users can create location anchors in your app, let them know to position the coordinates of each anchor within 0.05 degrees (~5 kilometers) of themselves and their device.

- The server prevents the location anchor’s position, such as in a large body of water.

## Topics

### Creating a Geo Anchor

convenience init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance?)

Initializes a location anchor with the given coordinate and altitude.

init(name: String, coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance)

Initializes a named location anchor with the given coordinates and altitude.

convenience init(name: String, coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance?)

Initializes a named location anchor with the given coordinates and altitude.

### Accessing Latitude and Longitude

var coordinate: CLLocationCoordinate2D

The lattitude and longitude of the anchor’s geographic location.

### Defining Altitude

var altitude: CLLocationDistance?

Vertical distance, in meters, between this anchor and sea level.

var altitudeSource: ARGeoAnchor.AltitudeSource

A record of the source from which an altitude came.

enum AltitudeSource

Options for setting a location anchor’s altitude.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- ARTrackable
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Geotracking

Tracking geographic locations in AR

Track specific geographic areas of interest and render them in an AR experience.

