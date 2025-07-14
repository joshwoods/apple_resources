

- Core Location
-  CLFloor 

Class

# CLFloor

The floor of a building on which the user’s device is located.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CLFloor
```

## Overview

A CLFloor object specifies the floor of the building on which the device is located. In places where floor information can be determined, a CLLocation object may include a floor object along with the regular location data.

You do not create instances of this class directly, nor should you subclass it.

## Topics

### Getting the floor level

var level: Int

The logical floor of the building.

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

class CLVisit

Information about the user’s location during a specific period of time.

class CLLocationSourceInformation

Information about the source that provides a location.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

class CLServiceSession

