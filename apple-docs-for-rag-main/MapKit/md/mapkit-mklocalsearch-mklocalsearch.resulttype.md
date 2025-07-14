

- MapKit
- MKLocalSearch
-  MKLocalSearch.ResultType 

Structure

# MKLocalSearch.ResultType

Options that indicate types of search results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
struct ResultType
```

## Overview

These options configure the types of search results you want to receive from MKLocalSearch.Request, including points of interest and addresses.

## Topics

### Creating the result type

init(rawValue: UInt)

Creates a search result type from the provided value.

### Specifying types of search results

static var address: MKLocalSearch.ResultType

A value that indicates that search results include addresses.

static var pointOfInterest: MKLocalSearch.ResultType

A value that indicates that search results include points of interest.

static var physicalFeature: MKLocalSearch.ResultType

A value that indicates that search results include physical features.

static var address: MKLocalSearch.ResultType

A value that indicates that search results include addresses.

static var pointOfInterest: MKLocalSearch.ResultType

A value that indicates that search results include points of interest.

static var physicalFeature: MKLocalSearch.ResultType

A value that indicates that search results include physical features.

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

class MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

