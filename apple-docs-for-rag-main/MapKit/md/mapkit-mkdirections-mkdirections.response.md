

- MapKit
- MKDirections
-  MKDirections.Response 

Class

# MKDirections.Response

The route information that Apple servers return in response to your request for directions.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Response
```

## Overview

You don’t create instances of this class directly. Instead, you initiate a request for directions by calling the calculate(completionHandler:) method of an MKDirections object. The completion handler you pass to that method receives an `MKDirections.Response` object with the results.

## Topics

### Getting the end points

var source: MKMapItem

The start point of the route.

var destination: MKMapItem

The end point of the route.

### Getting the route information

var routes: [MKRoute]

An array of route objects representing the directions between the start and end points.

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

class ETAResponse

The travel-time information that Apple servers return.

class MKRoute

A single route between a requested start and end point.

class Step

One portion of an overall route.

