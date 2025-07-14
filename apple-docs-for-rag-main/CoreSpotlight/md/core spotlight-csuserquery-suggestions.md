

- Core Spotlight
- CSUserQuery
-  suggestions 

Instance Property

# suggestions

An asynchronous sequence of suggested completions for the current query text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var suggestions: CSUserQuery.Suggestions { get }
```

## Discussion

Getting the value of this property starts the query and begins the delivery of suggestions. Typically, you get this property as part of a `for..in` loop to iterate over the suggestions and display them in your interface.

## See Also

### Executing the query automatically

var responses: CSUserQuery.Responses

The matching results and suggestions for the current query string.

struct Responses

An asynchronous sequence that contains the results and suggestions for a query string.

struct Suggestions

An asynchronous sequence that contains the suggested completions for a search string.

struct Item

A search result that the query returns in a response.

struct Suggestion

A suggested text completion for a query’s search term.

