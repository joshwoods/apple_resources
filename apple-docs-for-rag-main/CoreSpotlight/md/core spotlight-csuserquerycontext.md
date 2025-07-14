

- Core Spotlight
-  CSUserQueryContext 

Class

# CSUserQueryContext

The configuration details to apply to a user query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class CSUserQueryContext
```

## Mentioned in 

Building a search interface for your app

## Overview

Use an instance of `CSUserQueryContext` to configure the search parameters for a CSUserQuery object. This object stores configuration details that the query uses to modify the search results it delivers. For example, use this object to specify the maximum number of results or suggestions you want the query to return. You can also use it to enable or disable the ranking of results by Spotlight.

For information about search filters and other configurable query parameters, see the parent class CSSearchQueryContext.

## Topics

### Creating a query context

init(currentSuggestion: CSSuggestion?)

Creates a new query context object with an optional suggested search string.

### Configuring search options

var maxResultCount: Int

The maximum number of search results for the query to return.

var maxSuggestionCount: Int

The maximum number of suggested text completions for the query to return.

var disableSemanticSearch: Bool

A Boolean value that indicates whether to exclude semantic-based search results from the output.

### Configuring the ranked results behavior

var enableRankedResults: Bool

A Boolean value that indicates whether the query sorts results by their relevance.

var maxRankedResultCount: Int

The maximum number of ranked results to return during the query.

## Relationships

### Inherits From

- CSSearchQueryContext

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

### Queries

Building a search interface for your app

Add a search interface to your app to execute Spotlight queries and offer suggested text completions.

Searching for information in your app

Search for app-specific content and refine search results using predicates and filters.

class CSUserQuery

A type you use to initiate searches from your interface and offer suggested text completions.

class CSSearchQuery

A type you use to programmatically search the indexed app content.

class CSSearchQueryContext

The behavior configuration to use for a search query.

class CSSuggestion

The kind of suggestion to use in a query.

