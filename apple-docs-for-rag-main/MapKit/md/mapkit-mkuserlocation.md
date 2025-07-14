

- MapKit
-  MKUserLocation 

Class

# MKUserLocation

An annotation that reflects the user’s location on the map.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKUserLocation
```

## Mentioned in 

Converting a user’s location to a descriptive placemark

## Overview

You don’t create instances of this class directly. Instead, you retrieve an existing `MKUserLocation` object from the userLocation property of the map view that displays in your app.

## Topics

### Determining the user’s location

var location: CLLocation?

The location of the device.

var isUpdating: Bool

A Boolean value that indicates whether the map view is updating the user’s location.

var heading: CLHeading?

The heading of the user’s location.

### Accessing the user’s location annotation

var title: String?

The title to display for the user’s location annotation.

var subtitle: String?

The subtitle to display for the user’s location annotation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- NSObjectProtocol

## See Also

### User location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

class MKUserLocationView

A configurable annotation that shows the user’s location using the default MapKit style.

