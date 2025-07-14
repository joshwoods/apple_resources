

- MapKit
- MKLocalSearch
-  MKLocalSearch.Response 

Class

# MKLocalSearch.Response

The results from a map-based search.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Response
```

## Overview

You don’t create instances of this class directly. After initiating a map search using an MKLocalSearch object, MapKit passes an instance of this class to your completion handler.

## Topics

### Getting the search results

var mapItems: [MKMapItem]

An array of map items representing the search results.

var boundingRegion: MKCoordinateRegion

The map region that encloses the returned search results.

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

