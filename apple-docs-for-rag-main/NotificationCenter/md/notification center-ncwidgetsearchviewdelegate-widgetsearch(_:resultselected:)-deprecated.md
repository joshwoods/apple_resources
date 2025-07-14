

- Notification Center
- NCWidgetSearchViewDelegate
-  widgetSearch(\_:resultSelected:) Deprecated

Instance Method

# widgetSearch(\_:resultSelected:)

Tells the delegate that a user chose the specified search result.

macOS 10.10–11.0Deprecated

``` source
func widgetSearch(
    _ controller: NCWidgetSearchViewController,
    resultSelected object: Any
)
```

**Required**

Deprecated

Use WidgetKit instead.

## Parameters 

`controller`  

The widget’s search view controller.

`object`  

The object in the search view controller’s searchResults array that represents the search result chosen by the user.

## Discussion

When this method returns, the search view controller is dismissed.

## See Also

### Responding to User Choices

func widgetSearchTermCleared(NCWidgetSearchViewController)

Tells the delegate that a user cleared the search field.

**Required**

Deprecated

