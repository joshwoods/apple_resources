

- CarPlay
-  CPTrip 

Class

# CPTrip

An object that represents a journey between an origin and a destination.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPTrip
```

## Overview

A trip represents a journey consisting of an origin, a destination, and up to three route choices. Use CPRouteChoice to define each possible route choice.

You create trips after the user has selected a destination, and present up to twelve trip previews by calling showTripPreviews(_:textConfiguration:) on the map template.

You provide estimates for each trip using the map template’s updateEstimates(_:for:) method, and must update these estimates if the remaining time or distance changes.

## Topics

### Creating a Trip

init(origin: MKMapItem, destination: MKMapItem, routeChoices: [CPRouteChoice])

Creates a trip with an origin, destination, and route choices.

class CPRouteChoice

A possible route for a trip.

### Getting the Trip’s Origin and Destination

var origin: MKMapItem

The trip’s origin.

var destination: MKMapItem

The trip’s destination.

### Getting Route Choices

var routeChoices: [CPRouteChoice]

The list of route choices for the trip.

var destinationNameVariants: [String]?

An array of strings that represents the names of the destination for this trip, arranged from most to least preferred.

### Providing Additional Information

var userInfo: Any?

A custom object associated with the trip.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Getting the Trip

var trip: CPTrip

The trip associated with the navigation session.

