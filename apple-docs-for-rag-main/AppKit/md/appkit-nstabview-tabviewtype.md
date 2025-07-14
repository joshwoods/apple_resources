

- AppKit
- NSTabView
-  tabViewType 

Instance Property

# tabViewType

The tab type to display the tabs.

macOS

``` source
@MainActor
var tabViewType: NSTabView.TabType { get set }
```

## Discussion

The supported values for this property are listed in NSTabView.TabType. The default value of this property is NSTabView.TabType.topTabsBezelBorder.

## See Also

### Configuring the Tab Attributes

enum TabType

These constants specify the tab view’s type as used by the tabViewType property.

var tabPosition: NSTabView.TabPosition

enum TabPosition

var tabViewBorderType: NSTabView.TabViewBorderType

enum TabViewBorderType

