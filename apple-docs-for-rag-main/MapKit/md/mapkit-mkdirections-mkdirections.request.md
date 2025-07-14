

- MapKit
- MKDirections
-  MKDirections.Request 

Class

# MKDirections.Request

The start and end points of a route, along with the planned mode of transportation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Request
```

## Overview

You use an MKDirections.Request object when requesting or providing directions. If your app provides directions, use this class to decode the URL that the Maps app sends to you. If you need to request directions from Apple, pass an instance of this class to an MKDirections object. For example, an app that provides subway directions might request walking directions to and from relevant subway stations.

Prior to iOS 14, for apps that provide directions, you receive direction-related URLs in your app delegate’s application(_:open:options:)method. Upon receiving a URL, call the isDirectionsRequest(_:) method of this class to determine whether the URL relates to routing directions. If it does, create an instance of this class using the provided URL and extract the map items associated with the start and end points.

Note

Prior to iOS 14, to provide routing directions, your app needs to include special keys in its `Info.plist` file and be able to handle URLs that the Maps app sends to it. These keys indicate a special URL type that you app needs to handle. For information about how to implement this support, see Location and Maps Programming Guide.

## Topics

### Creating a directions request object

class func isDirectionsRequest(URL) -> Bool

Returns a Boolean value that indicates whether the specified URL contains a directions request.

init(contentsOfURL: URL)

Creates and returns a directions request object using the specified URL.

### Accessing the start and end points

var source: MKMapItem?

The starting point for routing directions.

var destination: MKMapItem?

The end point for routing directions.

### Specifying transportation options

var transportType: MKDirectionsTransportType

The type of conveyance that the directions apply to.

var highwayPreference: MKDirections.RoutePreference

The value that indicates whether the framework uses or avoids highways when providing directions.

var tollPreference: MKDirections.RoutePreference

The value that indicates whether the framework avoids routes that have tolls when providing directions.

enum RoutePreference

Options that modify how the framework selects routes when calculating directions.

var requestsAlternateRoutes: Bool

A Boolean value that indicates whether your app requests multiple routes when they’re available.

var departureDate: Date?

The departure date for the trip.

var arrivalDate: Date?

The arrival date for the trip.

### Constants

struct MKDirectionsTransportType

Constants that specify the type of conveyance to use.

### Launch options

let MKLaunchOptionsCameraKey: String

The virtual camera to use for viewing the map.

let MKLaunchOptionsDirectionsModeDefault: String

Directions that match the user’s preferred transportation type.

let MKLaunchOptionsDirectionsModeDriving: String

Driving directions between the specified start and end points.

let MKLaunchOptionsDirectionsModeKey: String

The mode of transportation.

let MKLaunchOptionsDirectionsModeTransit: String

Public transit directions between the specified start and end points.

let MKLaunchOptionsDirectionsModeWalking: String

Walking directions between the specified start and end points.

let MKLaunchOptionsMapCenterKey: String

The coordinate value on which to center the map.

let MKLaunchOptionsMapSpanKey: String

The amount of the map to display.

let MKLaunchOptionsMapTypeKey: String

The type of map (standard, satellite, or hybrid) to display.

let MKLaunchOptionsShowsTrafficKey: String

A Boolean value that indicates whether to display traffic information.

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

class Response

The route information that Apple servers return in response to your request for directions.

class ETAResponse

The travel-time information that Apple servers return.

class MKRoute

A single route between a requested start and end point.

class Step

One portion of an overall route.

