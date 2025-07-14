

- Notification Center
- NCWidgetSearchViewDelegate
-  widgetSearchTermCleared(\_:) Deprecated

Instance Method

# widgetSearchTermCleared(\_:)

Tells the delegate that a user cleared the search field.

macOS 10.10–11.0Deprecated

``` source
func widgetSearchTermCleared(_ controller: NCWidgetSearchViewController)
```

**Required**

Deprecated

Use WidgetKit instead.

## Parameters 

`controller`  

The widget’s search view controller.

## Discussion

When the delegate receives this message, it should stop the current search.

## See Also

### Responding to User Choices

func widgetSearch(NCWidgetSearchViewController, resultSelected: Any)

Tells the delegate that a user chose the specified search result.

**Required**

Deprecated

