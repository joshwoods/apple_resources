

- MapKit
- MKLocalSearch
-  init(request:) 

Initializer

# init(request:)

Creates and returns a search object with the specified parameters.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(request: MKLocalSearch.Request)
```

## Parameters 

`request`  

The search request information. This parameter can’t be `nil`.

## Return Value

An initialized search object.

## Discussion

This method stores a copy of the object in the `request` parameter. So, the object ignores any changes you make to your request object after calling this method.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a search request

init(request: MKLocalPointsOfInterestRequest)

Creates and returns a search object for fetching points of interest.

class Request

The parameters to use when searching for points of interest on the map.

struct ResultType

Options that indicate types of search results.

