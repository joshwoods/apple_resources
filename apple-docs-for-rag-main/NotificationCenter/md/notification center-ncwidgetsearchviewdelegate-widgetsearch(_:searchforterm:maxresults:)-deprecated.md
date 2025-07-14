

- Notification Center
- NCWidgetSearchViewDelegate
-  widgetSearch(\_:searchForTerm:maxResults:) Deprecated

Instance Method

# widgetSearch(\_:searchForTerm:maxResults:)

Asks the delegate to search using the specified term.

macOS 10.10–11.0Deprecated

``` source
func widgetSearch(
    _ controller: NCWidgetSearchViewController,
    searchForTerm searchTerm: String,
    maxResults max: Int
)
```

**Required**

Deprecated

Use WidgetKit instead.

## Parameters 

`controller`  

The widget’s search view controller.

`searchTerm`  

The term a user entered into the search field.

`max`  

The maximum number of results the search view controller can display.

## Discussion

The search view controller calls this method as soon as a user begins to type. If there is a maximum number of results the search view controller can display, it specifies this number in `max`. The delegate can use `max` to decide how many search results to return.

The delegate sets the search view controller’s searchResults property to the array of search result objects.

