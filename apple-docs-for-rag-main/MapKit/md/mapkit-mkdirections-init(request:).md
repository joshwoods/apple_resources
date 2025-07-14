

- MapKit
- MKDirections
-  init(request:) 

Initializer

# init(request:)

Creates and returns a directions object using the specified request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(request: MKDirections.Request)
```

## Parameters 

`request`  

The request object containing the start and end points of the route. This parameter must not be `nil`.

## Return Value

An initialized directions object.

## Discussion

After initializing your directions object, you must call the calculate(completionHandler:) or calculateETA(completionHandler:) method to perform the request.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a directions object

class Request

The start and end points of a route, along with the planned mode of transportation.

enum RoutePreference

Options that modify how the framework selects routes when calculating directions.

