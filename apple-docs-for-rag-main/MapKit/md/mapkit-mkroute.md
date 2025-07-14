

- MapKit
-  MKRoute 

Class

# MKRoute

A single route between a requested start and end point.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKRoute
```

## Overview

An `MKRoute` object defines the geometry for the route — that is, it contains line segments associated with specific map coordinates. A route object may also include other information, such as the name of the route, its distance, and the expected travel time.

You don’t create instances of this class directly. When you use an MKDirections object to request directions from Apple, the returned MKDirections.Response object contains the possible routes.

## Topics

### Getting the route geometry

var polyline: MKPolyline

The detailed route geometry.

var steps: [MKRoute.Step]

The array of steps that create the overall route.

class Step

One portion of an overall route.

### Getting additional route details

var name: String

The assigned name for the route.

var hasHighways: Bool

A Boolean value that indicates whether the route contains highways.

var hasTolls: Bool

A Boolean value that indicates whether the route has tolls.

var advisoryNotices: [String]

An array of advisory notice strings for the route.

var distance: CLLocationDistance

The route distance, in meters.

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var transportType: MKDirectionsTransportType

The overall route transport type.

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

class ETAResponse

The travel-time information that Apple servers return.

class Step

One portion of an overall route.

