

- Notification Center
- NCWidgetListViewController
-  minimumVisibleRowCount Deprecated

Instance Property

# minimumVisibleRowCount

The minimum number of visible rows to display.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var minimumVisibleRowCount: Int { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

Set this property to ensure that the widget’s list displays a minimum number of rows. The default value of this property is `0`.

If the value of `minimumVisibleRowCount` is nonzero and the number of items in contents is greater than this value, the list view controller displays the minimum number of rows and adds a “Show More…” button.

## See Also

### Customizing the List Appearance

var hasDividerLines: Bool

A Boolean value that indicates whether list displays divider lines between rows.

Deprecated

