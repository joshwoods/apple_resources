

- MapKit
-  MKLocalSearch 

Class

# MKLocalSearch

A utility object for initiating map-based searches and processing the results.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKLocalSearch
```

## Overview

Use an MKLocalSearch object to execute a single search request. You might use this class to search for addresses or points of interest on the map. Upon completion of the request, the object delivers the results to the completion handler that you provide.

## Topics

### Creating a search request

init(request: MKLocalSearch.Request)

Creates and returns a search object with the specified parameters.

init(request: MKLocalPointsOfInterestRequest)

Creates and returns a search object for fetching points of interest.

class Request

The parameters to use when searching for points of interest on the map.

struct ResultType

Options that indicate types of search results.

### Performing the search

func start(completionHandler: (MKLocalSearch.Response?, (any Error)?) -> Void)

Starts the search and delivers the results to the specified completion handler.

typealias CompletionHandler

A completion handler block for a search operation.

var isSearching: Bool

A Boolean value that indicates whether the search is in progress.

func cancel()

Cancels an in-progress search operation.

### Getting search results

class Response

The results from a map-based search.

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

### Local search

Interacting with nearby points of interest

Provide automatic search completions for a partial search query, search the map for relevant locations nearby, and retrieve details for selected points of interest.

enum MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

struct ResultType

Options that indicate types of search results.

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

class MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

