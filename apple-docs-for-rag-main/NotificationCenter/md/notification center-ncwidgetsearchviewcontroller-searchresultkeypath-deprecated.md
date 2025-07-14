

- Notification Center
- NCWidgetSearchViewController
-  searchResultKeyPath Deprecated

Instance Property

# searchResultKeyPath

A key path for the string property to display for each object in the search results array.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var searchResultKeyPath: String? { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

The search view controller uses the key path to find the textual description of each object in searchResults. The default value of this property is “description”.

## See Also

### Displaying Search Results

var searchResults: [Any]?

An array of search results.

Deprecated

