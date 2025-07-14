

- Notification Center
- NCWidgetListViewController
-  contents Deprecated

Instance Property

# contents

An array of objects to display in the list view.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var contents: [Any] { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

The list view controller asks its delegate for a new content view controller for each object in `contents`, and sets the representedObject of the newly created content view controller accordingly. To optimize content resetting, the list view controller may reuse content view controllers for identical objects that already exist in `contents`.

## See Also

### Accessing Content

func row(for: NSViewController) -> Int

Returns the row represented by the specified content view controller.

Deprecated

func viewController(atRow: Int, makeIfNecessary: Bool) -> NSViewController

Returns the content view controller associated with the specified row, or a new content view controller if desired.

Deprecated

