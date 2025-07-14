

- SwiftUI
- EnvironmentValues
-  tabBarPlacement 

Instance Property

# tabBarPlacement

The current placement of the tab bar.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var tabBarPlacement: TabBarPlacement? { get }
```

## Discussion

Note that this value is only set within the content views of a TabView.

A `nil` value corresponds to an undefined placement.

## See Also

### Configuring a tab bar

func tabViewSidebarHeader&lt;Content>(content: () -> Content) -> some View

Adds a custom header to the sidebar of a tab view.

func tabViewSidebarFooter&lt;Content>(content: () -> Content) -> some View

Adds a custom footer to the sidebar of a tab view.

func tabViewSidebarBottomBar&lt;Content>(content: () -> Content) -> some View

Adds a custom bottom bar to the sidebar of a tab view.

struct AdaptableTabBarPlacement

A placement for tabs in a tab view using the adaptable sidebar style.

struct TabBarPlacement

A placement for tabs in a tab view.

var isTabBarShowingSections: Bool

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

