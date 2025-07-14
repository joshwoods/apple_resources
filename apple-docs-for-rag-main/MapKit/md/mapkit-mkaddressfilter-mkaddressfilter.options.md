

- MapKit
- MKAddressFilter
-  MKAddressFilter.Options 

Structure

# MKAddressFilter.Options

A structure that contains options for filtering results in a search.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Options
```

## Topics

### Creating a filter result

init(rawValue: UInt)

Creates a filter options object.

### Getting search filter options

static var administrativeArea: MKAddressFilter.Options

The primary administrative divisions of countries or regions.

static var country: MKAddressFilter.Options

Countries and regions.

static var locality: MKAddressFilter.Options

Local administrative divisions, postal cities, and populated places.

static var postalCode: MKAddressFilter.Options

An address code for mail sorting and delivery.

static var subAdministrativeArea: MKAddressFilter.Options

The secondary administrative divisions of countries or regions.

static var subLocality: MKAddressFilter.Options

Local administrative subdivisions, postal city subdistricts, and neighborhoods.

static var administrativeArea: MKAddressFilter.Options

The primary administrative divisions of countries or regions.

static var country: MKAddressFilter.Options

Countries and regions.

static var locality: MKAddressFilter.Options

Local administrative divisions, postal cities, and populated places.

static var postalCode: MKAddressFilter.Options

An address code for mail sorting and delivery.

static var subAdministrativeArea: MKAddressFilter.Options

The secondary administrative divisions of countries or regions.

static var subLocality: MKAddressFilter.Options

Local administrative subdivisions, postal city subdistricts, and neighborhoods.

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

