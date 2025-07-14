

- Quartz
- IKFilterBrowserPanel
-  filterName() 

Instance Method

# filterName()

Returns the name of the filter that is currently selected in the filter browser.

macOS 10.4+

``` source
@MainActor
func filterName() -> String!
```

## Return Value

The name of the currently selected filter.

## Discussion

Use this method in response to the notifications IKFilterBrowserFilterSelectedNotification or IKFilterBrowserFilterDoubleClickNotification, or after the user makes a choice in a dialog.

