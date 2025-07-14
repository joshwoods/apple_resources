

- Notification Center
- NCWidgetSearchViewController
-  searchResults Deprecated

Instance Property

# searchResults

An array of search results.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var searchResults: [Any]? { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

The delegate updates this property with the results of the search. For each object in `searchResults`, the search view controller uses the searchResultKeyPath property to find the description of the object to display in search view.

When a user chooses an item in the search view’s results list, the search view controller calls widgetSearch(_:resultSelected:) on its delegate. If the widget presented the search view using `presentViewControllerInWidget:`, this action causes the search view to be dismissed by `dismissViewController:`.

## See Also

### Displaying Search Results

var searchResultKeyPath: String?

A key path for the string property to display for each object in the search results array.

Deprecated

