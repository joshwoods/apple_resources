

- Core Location
-  CLRegion 

Class

# CLRegion

A base class representing an area that can be monitored.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+watchOS 2.0+

``` source
class CLRegion
```

## Overview

This is an abstract base class. Instantiate one of the provided subclasses that define specific types of regions. After you create a region, register it with a CLLocationManager object with the startMonitoring(for:) method. The location manager generates appropriate events whenever the user crosses the boundaries of the region.

## Topics

### Getting the region identifier

var identifier: String

The identifier for the region object.

### Specifying the notification conditions

var notifyOnEntry: Bool

A Boolean indicating that notifications are generated upon entry into the region.

var notifyOnExit: Bool

A Boolean indicating that notifications are generated upon exit from the region.

### Deprecated

init(circularRegionWithCenter: CLLocationCoordinate2D, radius: CLLocationDistance, identifier: String)

Initializes and returns a region object defining a circular area.

Deprecated

func contains(CLLocationCoordinate2D) -> Bool

Returns a Boolean value indicating whether the region contains the specified coordinate.

Deprecated

var center: CLLocationCoordinate2D

The center point of the region.

Deprecated

var radius: CLLocationDistance

The radius (measured in meters) that defines the region’s outer boundary.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLBeaconRegion
- CLCircularRegion

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

### Region monitoring

Monitoring the user’s proximity to geographic regions

Use condition monitoring to determine when the user enters or leaves a geographic region.

