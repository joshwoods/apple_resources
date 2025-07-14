

- Notification Center
- NCWidgetListViewDelegate
-  widgetList(\_:viewControllerForRow:) Deprecated

Instance Method

# widgetList(\_:viewControllerForRow:)

Asks the delegate for a content view controller for the specified row.

macOS 10.10–11.0Deprecated

``` source
func widgetList(
    _ list: NCWidgetListViewController,
    viewControllerForRow row: Int
) -> NSViewController
```

**Required**

Deprecated

Use WidgetKit instead.

## Parameters 

`list`  

The widget’s list view controller that is requesting this content view controller.

`row`  

The number of the row in the list.

## Return Value

A custom view controller to manage the content in the specified row.

