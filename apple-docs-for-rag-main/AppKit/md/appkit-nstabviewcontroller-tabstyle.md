

- AppKit
- NSTabViewController
-  tabStyle 

Instance Property

# tabStyle

The style used to display the tabs.

macOS 10.10+

``` source
@MainActor
var tabStyle: NSTabViewController.TabStyle { get set }
```

## Discussion

The default value of this property is NSTabViewController.TabStyle.segmentedControlOnTop. Changing the style at runtime updates the appearance of the tab view controller interface.

## See Also

### Configuring the Tab View

var tabView: NSTabView

The tab view that manages the views of the interface.

var transitionOptions: NSViewController.TransitionOptions

The animation options to use when switching between tabs.

var canPropagateSelectedChildViewControllerTitle: Bool

A Boolean value indicating whether the tab view controller gets its title from the selected child view controller.

