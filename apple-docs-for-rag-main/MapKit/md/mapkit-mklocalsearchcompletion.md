

- MapKit
-  MKLocalSearchCompletion 

Class

# MKLocalSearchCompletion

A fully formed string that completes a partial string.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
class MKLocalSearchCompletion
```

## Overview

You don’t create instances of this class directly. Instead, you use an MKLocalSearchCompleter to initiate a search based on a set of partial search strings. That object stores any matches in its results property. Retrieve any `MKLocalSearchCompletion` objects from that property and display the search terms in your interface, or use one to initiate a search for content based on that search term.

When displaying text completions for a partial search term in your user interface, you might want to use a bold version of a font or add some other highlighting to the portion of the completion string that causes it to match the partial search term. To help you add this styling, the completion object includes highlight ranges for the title and subtitle strings.

## Topics

### Getting the search completions

var title: String

The title string associated with the point of interest.

var subtitle: String

The subtitle (if any) associated with the point of interest.

var titleHighlightRanges: [NSValue]

The ranges of characters to highlight in the title string.

var subtitleHighlightRanges: [NSValue]

The ranges of characters to highlight in the subtitle string.

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

class MKLocalPointsOfInterestRequest

A structured request to use when searching for points of interest.

