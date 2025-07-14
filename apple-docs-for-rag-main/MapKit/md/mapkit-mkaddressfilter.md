

- MapKit
-  MKAddressFilter 

Class

# MKAddressFilter

An object that filters which address options to include or exclude in search results.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class MKAddressFilter
```

## Overview

Use this object to filter search results by criteria, such as country, region, and municipality. See MKAddressFilter.Options for more information.

## Topics

### Creating a filter

init(excluding: MKAddressFilter.Options)

Creates an address filter with options for excluding results in a search.

init(including: MKAddressFilter.Options)

Creates an address filter with options for including results in a search.

### Filtering results

struct Options

A structure that contains options for filtering results in a search.

class var excludingAll: MKAddressFilter

A list of categories to exclude from a search.

class var includingAll: MKAddressFilter

A list of categories to include in a search.

func excludes(MKAddressFilter.Options) -> Bool

Indicates whether options are excluded from filtering.

func includes(MKAddressFilter.Options) -> Bool

Indicates whether options are included for filtering.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

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

struct ResultType

Options that indicate types of search completions.

class MKLocalSearchCompleter

A utility object for generating a list of completion strings based on a partial search string that you provide.

class MKLocalSearchCompletion

A fully formed string that completes a partial string.

class MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

