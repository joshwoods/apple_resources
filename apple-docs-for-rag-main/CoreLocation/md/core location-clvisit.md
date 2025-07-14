

- Core Location
-  CLVisit 

Class

# CLVisit

Information about the user’s location during a specific period of time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
class CLVisit
```

## Overview

A CLVisit object encapsulates information about places that the user has been. Visit objects are created by the system and delivered by the CLLocationManager object to its delegate after you start the delivery of events. The visit includes the location where the visit occurred and information about the arrival and departure times as relevant. You do not create visit objects directly, nor should you subclass CLVisit.

Visit objects contain as much information about the visit as possible but may not always include both the arrival and departure times. For example, when the user arrives at a location, the system may send an event with only an arrival time. When the user departs a location, the event can contain both the arrival time (if your app was monitoring visits prior to the user’s arrival) and the departure time.

## Topics

### Getting the location

var coordinate: CLLocationCoordinate2D

The geographical coordinate information.

var horizontalAccuracy: CLLocationAccuracy

The horizontal accuracy (in meters) of the specified coordinate.

### Getting the visit duration

var arrivalDate: Date

The approximate time at which the user arrived at the specified location.

var departureDate: Date

The approximate time at which the user left the specified location.

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

### Location updates

Getting the current location of a device

Start location services and provide information the system needs to optimize power usage for those services.

Handling location updates in the background

Configure your app to receive location updates when it isn’t running in the foreground.

Creating a location push service extension

Add and configure an extension to enable your location-sharing app to access a user’s location in response to a request from another user.

class CLLocation

The latitude, longitude, and course information reported by the system.

struct CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

class CLFloor

The floor of a building on which the user’s device is located.

class CLLocationSourceInformation

Information about the source that provides a location.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

class CLServiceSession

