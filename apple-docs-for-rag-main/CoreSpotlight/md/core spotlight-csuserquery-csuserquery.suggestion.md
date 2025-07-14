

- Core Spotlight
- CSUserQuery
-  CSUserQuery.Suggestion 

Structure

# CSUserQuery.Suggestion

A suggested text completion for a query’s search term.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct Suggestion
```

## Mentioned in 

Building a search interface for your app

## Discussion

When executing its query, a CSUserQuery object returns both results and suggestions for text completions of the current term. Use the suggestion property of this structure to get one of the suggestions to display in your app’s interface and use in a new query.

## Topics

### Instance Properties

var suggestion: CSSuggestion

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

struct Item

A search result that the query returns in a response.

