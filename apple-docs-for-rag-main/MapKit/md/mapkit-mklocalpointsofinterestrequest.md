

- MapKit
-  MKLocalPointsOfInterestRequest 

Class

# MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MKLocalPointsOfInterestRequest
```

## Overview

You create an MKLocalPointsOfInterestRequest to fetch points of interest within a rectangular bounding box or circular area.

To leverage the phone’s viewport to request points of interest, create a request with a rectangular bounding box using an MKCoordinateRegion. The request fetches points of interest within the rectangular region.

To retrieve points of interest nearby or “around the user,” create a request with a circular area defined by CLLocationCoordinate2D and a CLLocationDistance in meters. The fetch returns points of interest up to the maximum distance defined by maxRadius.

You may optionally specifying an MKPointOfInterestFilter describing categories to include or exclude. The default behavior of the fetch returns all points of interest.

## Topics

### Creating a point of interest request

init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates a points of interest search request centered on the provided coordinate with the provided radius.

init(coordinateRegion: MKCoordinateRegion)

Creates a points of interest search request based on existing region.

### Configuring the request parameters

var region: MKCoordinateRegion

The region of the bounding box of the request provided or the derived bounding box of the circle created by the radius.

var coordinate: CLLocationCoordinate2D

The center of the point of request as latitude and longitude.

var radius: CLLocationDistance

The distance provided in meters or the longest distance derived from the center point to the region’s bounding box.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists points of interest categories to include or exclude.

### Getting the maximum radius

class let maxRadius: CLLocationDistance

The maximum distance respected for fetching points of interest from the center of the region.

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

### Local search

Interacting with nearby points of interest

Provide automatic search completions for a partial search query, search the map for relevant locations nearby, and retrieve details for selected points of interest.

enum MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

struct ResultType

Options that indicate types of search results.

class MKLocalSearch

A utility object for initiating map-based searches and processing the results.

struct Options

A structure that contains options for filtering results in a search.

class MKAddressFilter

An object that filters which address options to include or exclude in search results.

struct ResultType

Options that indicate types of search completions.

class MKLocalSearchCompleter

A utility object for generating a list of completion strings based on a partial search string that you provide.

class MKLocalSearchCompletion

A fully formed string that completes a partial string.

