

- Core Spotlight
- CSSearchQuery
-  results 

Instance Property

# results

The results that match the current query string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var results: CSSearchQuery.Results { get }
```

## Mentioned in 

Searching for information in your app

## Discussion

Getting the value of this property starts the query automatically and begins the delivery of results. Typically, you get this property as part of a `for..in` loop and iterate over the responses, as shown in the following example:

```
var results: [String] = []
let query = CSSearchQuery(queryString: searchText, queryContext: queryContext)

for try await element in query.results {
    if let title = element.item.attributeSet.title {
    results.append(title)
    }
}
```

## See Also

### Executing the query automatically

struct Results

An asynchronous sequence that contains the results that match the query string.

