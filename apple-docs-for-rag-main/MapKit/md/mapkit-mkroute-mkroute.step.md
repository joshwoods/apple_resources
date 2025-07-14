

- MapKit
- MKRoute
-  MKRoute.Step 

Class

# MKRoute.Step

One portion of an overall route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Step
```

## Overview

Each `MKRoute.Step` object corresponds to a single instruction that the person needs to follow when navigating between two points. For example, a step might involve following a single road until continuing along the route requires a turn.

You don’t create instances of this class directly. An MKRoute object contains the `MKRoute.Step` objects associated with a route. For more information about requesting directions, see MKDirections.

## Topics

### Getting the step geometry

var polyline: MKPolyline

The detailed step geometry.

### Getting additional step details

var instructions: String

The written instructions for following the path that the step represents.

var notice: String?

Additional notices that apply to the step.

var distance: CLLocationDistance

The step distance, in meters.

var transportType: MKDirectionsTransportType

The transport type of the step.

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

class MKRoute

A single route between a requested start and end point.

