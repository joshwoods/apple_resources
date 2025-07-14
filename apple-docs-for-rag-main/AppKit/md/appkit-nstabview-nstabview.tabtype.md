

- AppKit
- NSTabView
-  NSTabView.TabType 

Enumeration

# NSTabView.TabType

These constants specify the tab view’s type as used by the tabViewType property.

macOS

``` source
enum TabType
```

## Topics

### Constants

case topTabsBezelBorder

The view includes tabs on the top of the view and has a bezeled border (the default).

case noTabsBezelBorder

The view does not include tabs and has a bezeled border.

case noTabsLineBorder

The view does not include tabs and has a lined border.

case noTabsNoBorder

The view does not include tabs and has no border.

case bottomTabsBezelBorder

Tabs are on the bottom of the view with a bezeled border.

case leftTabsBezelBorder

Tabs are on the left of the view with a bezeled border.

case rightTabsBezelBorder

Tabs are on the right of the view with a bezeled border.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the Tab Attributes

var tabViewType: NSTabView.TabType

The tab type to display the tabs.

var tabPosition: NSTabView.TabPosition

enum TabPosition

var tabViewBorderType: NSTabView.TabViewBorderType

enum TabViewBorderType

