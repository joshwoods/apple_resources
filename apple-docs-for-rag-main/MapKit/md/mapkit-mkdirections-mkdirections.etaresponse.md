

- MapKit
- MKDirections
-  MKDirections.ETAResponse 

Class

# MKDirections.ETAResponse

The travel-time information that Apple servers return.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class ETAResponse
```

## Overview

You don’t create instances of this class directly. Instead, you initiate a request for the travel time by calling the calculateETA(completionHandler:) method of an MKDirections object. The completion handler you pass to that method receives an `MKDirections.ETAResponse` object with the results.

## Topics

### Getting the end points

var source: MKMapItem

The start point of the route.

var destination: MKMapItem

The end point of the route.

### Getting the travel information

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var expectedDepartureDate: Date

The expected departure time.

var expectedArrivalDate: Date

The expected arrival time.

var distance: CLLocationDistance

The expected travel distance, in meters.

var transportType: MKDirectionsTransportType

The type of conveyance to use for determining the travel time.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Directions

class MKDirections

A utility object that computes directions and travel-time information based on the route information you provide.

class Request

The start and end points of a route, along with the planned mode of transportation.

class Response

The route information that Apple servers return in response to your request for directions.

class MKRoute

A single route between a requested start and end point.

class Step

One portion of an overall route.

