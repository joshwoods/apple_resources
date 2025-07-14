

- AppKit
- NSTabViewController
-  canPropagateSelectedChildViewControllerTitle 

Instance Property

# canPropagateSelectedChildViewControllerTitle

A Boolean value indicating whether the tab view controller gets its title from the selected child view controller.

macOS 10.10+

``` source
@MainActor
var canPropagateSelectedChildViewControllerTitle: Bool { get set }
```

## Discussion

When this property is true and the tab view controller’s own title is `nil`, the tab view controller gets its title from the title property of the selected child view controller. When this property is false, the tab view controller always provides the title, which may be `nil`. The default value of this property is true.

## See Also

### Configuring the Tab View

var tabStyle: NSTabViewController.TabStyle

The style used to display the tabs.

var tabView: NSTabView

The tab view that manages the views of the interface.

var transitionOptions: NSViewController.TransitionOptions

The animation options to use when switching between tabs.

