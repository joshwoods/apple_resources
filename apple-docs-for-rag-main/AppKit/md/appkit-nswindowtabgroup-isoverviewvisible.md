

- AppKit
- NSWindowTabGroup
-  isOverviewVisible 

Instance Property

# isOverviewVisible

A Boolean value indicating if the tab overview is currently displayed.

macOS 10.13+

``` source
var isOverviewVisible: Bool { get set }
```

## Discussion

The tab overview provides a visual overview of the windows that make up a tabbing group. This property indicates whether the tab overview is currently displayed. Setting the property either shows or hides the overview.

You can monitor this property for changes using key-value observing.

## See Also

### Related Documentation

func toggleTabOverview(Any?)

Shows or hides the tab overview.

### Configuring the Tab User Interface

var isTabBarVisible: Bool

A Boolean value indicating whether the tabbed window group currently displays a tab bar.

