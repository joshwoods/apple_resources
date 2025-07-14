

- Core Spotlight
- CSUserQuery
-  CSUserQuery.Item 

Structure

# CSUserQuery.Item

A search result that the query returns in a response.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct Item
```

## Topics

### Instance Properties

var item: CSSearchableItem

## Relationships

### Conforms To

- Comparable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Executing the query automatically

var responses: CSUserQuery.Responses

The matching results and suggestions for the current query string.

var suggestions: CSUserQuery.Suggestions

An asynchronous sequence of suggested completions for the current query text.

struct Responses

An asynchronous sequence that contains the results and suggestions for a query string.

struct Suggestions

An asynchronous sequence that contains the suggested completions for a search string.

struct Suggestion

A suggested text completion for a query’s search term.

