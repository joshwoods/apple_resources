

- Core Spotlight
- CSUserQuery
-  responses 

Instance Property

# responses

The matching results and suggestions for the current query string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var responses: CSUserQuery.Responses { get }
```

## Mentioned in 

Building a search interface for your app

## Discussion

Getting the value of this property starts the query and begins the delivery of responses. Typically, you get this property as part of a `for..in` loop to iterate over the responses, as shown in the following example:

```
var results: [CSUserQuery.Item] = []
var suggestions: [CSUserQuery.Suggestion] = []
let query = CSUserQuery(userQueryString: searchText, userQueryContext: queryContext)

for try await element in query.responses {
    switch(element) {
        case .item(let item):
            self.results.append(item)
            break
        case .suggestion(let suggestion):
            self.suggestions.append(suggestion)
            break
        @unknown default:
            break
    }
}
```

## See Also

### Executing the query automatically

var suggestions: CSUserQuery.Suggestions

An asynchronous sequence of suggested completions for the current query text.

struct Responses

An asynchronous sequence that contains the results and suggestions for a query string.

struct Suggestions

An asynchronous sequence that contains the suggested completions for a search string.

struct Item

A search result that the query returns in a response.

struct Suggestion

A suggested text completion for a query’s search term.

