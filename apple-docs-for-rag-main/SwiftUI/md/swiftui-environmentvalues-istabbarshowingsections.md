

- SwiftUI
- EnvironmentValues
-  isTabBarShowingSections 

Instance Property

# isTabBarShowingSections

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var isTabBarShowingSections: Bool { get }
```

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

var tabBarPlacement: TabBarPlacement?

The current placement of the tab bar.

struct TabBarPlacement

A placement for tabs in a tab view.

