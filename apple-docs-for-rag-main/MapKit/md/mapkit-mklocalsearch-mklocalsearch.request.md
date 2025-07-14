

- MapKit
- MKLocalSearch
-  MKLocalSearch.Request 

Class

# MKLocalSearch.Request

The parameters to use when searching for points of interest on the map.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Request
```

## Overview

You create an MKLocalSearch.Request object when you want to search for map locations based on a natural language string. For example, if your interface allows the user to type in addresses, place the typed text in this object and pass it to an MKLocalSearch object to begin the search process. When specifying your search strings, include a map region to narrow the search results to the specified geographical area.

When creating an MKLocalSearch.Request object yourself, set the naturalLanguageQuery property to an appropriate search string, as in the following example:

- Swift
- Objective-C

```
let searchRequest = MKLocalSearch.Request()
searchRequest.naturalLanguageQuery = "coffee"

// Set the region to an associated map view's region.
searchRequest.region = myMapView.region

let search = MKLocalSearch(request: searchRequest)
search.start { (response, error) in
    guard let response = response else {
        // Handle the error.
    }

    for item in response.mapItems {
        if let name = item.name,
            let location = item.placemark.location {
            print("\(name): \(location.coordinate.latitude),\(location.coordinate.longitude)")
        }
    }
}
```

```
```

If your app uses an MKLocalSearchCompleter object to implement autocomplete support for user-supplied search strings, initialize your search request using the search completion that the user selects. In that case, use the init(completion:) method instead of the init() method to initialize your search request object. The completion object automatically provides the value for the naturalLanguageQuery property.

## Topics

### Creating a local search request

init()

Creates a local search request.

init(completion: MKLocalSearchCompletion)

Creates and returns a search request based on the specified search completion data.

### Configuring the search parameters

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var naturalLanguageQuery: String?

A string containing the desired search item.

var region: MKCoordinateRegion

A map region that provides a hint as to where to search.

static var physicalFeature: MKLocalSearch.ResultType

A value that indicates that search results include physical features.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point-of-interest categories to include or exclude in search results.

var regionPriority: MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

var resultTypes: MKLocalSearch.ResultType

The types of items to include in the search results.

typealias ResultType

Options that indicate types of search results.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a search request

init(request: MKLocalSearch.Request)

Creates and returns a search object with the specified parameters.

init(request: MKLocalPointsOfInterestRequest)

Creates and returns a search object for fetching points of interest.

struct ResultType

Options that indicate types of search results.

