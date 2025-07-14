

- Notification Center
- NCWidgetListViewController
-  row(for:) Deprecated

Instance Method

# row(for:)

Returns the row represented by the specified content view controller.

macOS 10.10–11.0Deprecated

``` source
@MainActor
func row(for viewController: NSViewController) -> Int
```

Deprecated

Use WidgetKit instead.

## Parameters 

`viewController`  

The content view controller created by the delegate to display the object in the row.

## Return Value

The row represented by the content view controller.

## See Also

### Accessing Content

var contents: [Any]

An array of objects to display in the list view.

Deprecated

func viewController(atRow: Int, makeIfNecessary: Bool) -> NSViewController

Returns the content view controller associated with the specified row, or a new content view controller if desired.

Deprecated

