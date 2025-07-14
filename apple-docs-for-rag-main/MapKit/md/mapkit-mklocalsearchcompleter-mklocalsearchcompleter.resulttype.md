

- MapKit
- MKLocalSearchCompleter
-  MKLocalSearchCompleter.ResultType 

Structure

# MKLocalSearchCompleter.ResultType

Options that indicate types of search completions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
struct ResultType
```

## Topics

### Type properties

static var address: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes address completions in the result.

static var pointOfInterest: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes point-of-interest completions in the result.

static var physicalFeature: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes physical feature completions in the result.

static var query: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes query completions in the result.

### Initializers

init(rawValue: UInt)

Creates a direction transport type using a raw unsigned integer value.

static var address: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes address completions in the result.

static var pointOfInterest: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes point-of-interest completions in the result.

static var physicalFeature: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes physical feature completions in the result.

static var query: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes query completions in the result.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

class MKLocalSearchCompleter

A utility object for generating a list of completion strings based on a partial search string that you provide.

class MKLocalSearchCompletion

A fully formed string that completes a partial string.

class MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

