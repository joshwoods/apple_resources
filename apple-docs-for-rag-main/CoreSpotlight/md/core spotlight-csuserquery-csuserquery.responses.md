

- Core Spotlight
- CSUserQuery
-  CSUserQuery.Responses 

Structure

# CSUserQuery.Responses

An asynchronous sequence that contains the results and suggestions for a query string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct Responses
```

## Discussion

A `CSUserQuery/Responses-struct` structure contains the results of a query. Fetch this structure from the responses property of your query object to execute the query automatically and begin the delivery of the results. Each element that this structure returns to you is either a search result or a suggested completion of the current search text. Check the element type and handle it accordingly.

For more information about how to use this structure, see the responses property.

## Topics

### Getting the response type

enum Response

### Iterating over the responses

struct Iterator

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Executing the query automatically

var responses: CSUserQuery.Responses

The matching results and suggestions for the current query string.

var suggestions: CSUserQuery.Suggestions

An asynchronous sequence of suggested completions for the current query text.

struct Suggestions

An asynchronous sequence that contains the suggested completions for a search string.

struct Item

A search result that the query returns in a response.

struct Suggestion

A suggested text completion for a query’s search term.

