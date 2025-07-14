

- Notification Center
- NCWidgetSearchViewController
-  searchDescription Deprecated

Instance Property

# searchDescription

A localized description of the nature of the search.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var searchDescription: String? { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

The search description is displayed above the search field. If appropriate, the search display controller can change the description to reflect the current status of the search. The default value of this property is “Search”.

## See Also

### Displaying the Search Interface

var searchResultsPlaceholderString: String?

A localized phrase displayed in the results list when no search results are available.

Deprecated

