

- Notification Center
- NCWidgetListViewController
-  viewController(atRow:makeIfNecessary:) Deprecated

Instance Method

# viewController(atRow:makeIfNecessary:)

Returns the content view controller associated with the specified row, or a new content view controller if desired.

macOS 10.10–11.0Deprecated

``` source
@MainActor
func viewController(
    atRow row: Int,
    makeIfNecessary makeIfNecesary: Bool
) -> NSViewController
```

Deprecated

Use WidgetKit instead.

## Parameters 

`row`  

The row in the list.

`makeIfNecesary`  

Specify true to create a new content view controller if none exists or false to reuse an existing row.

## Return Value

The content view controller associated with the specified row, if one exists. Returns `nil` if the row doesn’t have a content view controller and you don’t want to create one.

## See Also

### Accessing Content

var contents: [Any]

An array of objects to display in the list view.

Deprecated

func row(for: NSViewController) -> Int

Returns the row represented by the specified content view controller.

Deprecated

