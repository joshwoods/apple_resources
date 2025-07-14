

- AppKit
- NSTabViewController
- NSTabViewController.TabStyle
-  NSTabViewController.TabStyle.unspecified 

Case

# NSTabViewController.TabStyle.unspecified

A style that indicates the tab view controller does not provide the tab selection UI. Your app provides the control (such as an NSSegmentedControl or NSPopUpButton) for navigating between tabs. You can bind an existing control to the tab view controller object so that interactions with the control automatically change tabs.

macOS 10.10+

``` source
case unspecified
```

## See Also

### Constants

case segmentedControlOnTop

A style that displays a segmented control along the top edge of the tab view interface. Access the configuration of the tab items through the tab view, which you can get from the tabView property.

case segmentedControlOnBottom

A style that displays a segmented control along the bottom edge of the tab view interface. Access the configuration of the tab items through the tab view, which you can get from the tabView property.

case toolbar

A style that automatically adds any tabs to the window’s toolbar. The tab view controller takes control of the window’s toolbar and sets itself as the toolbar’s delegate. Customization of the toolbar is handled using the methods in Responding to Toolbar Events.

