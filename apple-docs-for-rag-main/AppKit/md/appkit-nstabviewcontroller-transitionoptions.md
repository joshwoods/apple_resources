

- AppKit
- NSTabViewController
-  transitionOptions 

Instance Property

# transitionOptions

The animation options to use when switching between tabs.

macOS 10.10+

``` source
@MainActor
var transitionOptions: NSViewController.TransitionOptions { get set }
```

## Discussion

By default, this property is set to the crossfade and allowUserInteraction options.

The tab view controller uses the transition(from:to:options:completionHandler:) method to perform transitions between tabs. For more information about how transitions happen, see the description of that method.

## See Also

### Configuring the Tab View

var tabStyle: NSTabViewController.TabStyle

The style used to display the tabs.

var tabView: NSTabView

The tab view that manages the views of the interface.

var canPropagateSelectedChildViewControllerTitle: Bool

A Boolean value indicating whether the tab view controller gets its title from the selected child view controller.

