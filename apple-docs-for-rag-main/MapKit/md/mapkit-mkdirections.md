

- MapKit
-  MKDirections 

Class

# MKDirections

A utility object that computes directions and travel-time information based on the route information you provide.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKDirections
```

## Mentioned in 

Enabling Maps capability in Xcode

## Overview

You use an `MKDirections` object to ask the Apple servers to provide walking or driving directions for a route, which you specify using an MKDirections.Request object. After making a request, MapKit delivers the results asynchronously to the completion handler that you provide. You can also get the estimated travel time for the route.

Each `MKDirections` object handles a single request for directions, although you can cancel and restart that request as needed. You can create multiple instances of this class and process different route requests at the same time, but make requests only when you plan to present the corresponding route information to the user. Apps may receive an MKError.Code.loadingThrottled error if the device makes too many requests in too short a time period.

## Topics

### Creating a directions object

init(request: MKDirections.Request)

Creates and returns a directions object using the specified request.

class Request

The start and end points of a route, along with the planned mode of transportation.

enum RoutePreference

Options that modify how the framework selects routes when calculating directions.

### Getting the directions

func calculate(completionHandler: MKDirections.DirectionsHandler)

Begins calculating the requested route information asynchronously.

typealias DirectionsHandler

The block to use for processing the requested route information.

class Response

The route information that Apple servers return in response to your request for directions.

### Getting the ETA

func calculateETA(completionHandler: MKDirections.ETAHandler)

Begins calculating the requested travel-time information asynchronously.

typealias ETAHandler

The block to use for processing travel-time information.

class ETAResponse

The travel-time information that Apple servers return.

### Managing the request

func cancel()

Cancels a pending request.

var isCalculating: Bool

A Boolean value that indicates whether a request is in process.

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

class Request

The start and end points of a route, along with the planned mode of transportation.

class Response

The route information that Apple servers return in response to your request for directions.

class ETAResponse

The travel-time information that Apple servers return.

class MKRoute

A single route between a requested start and end point.

class Step

One portion of an overall route.

