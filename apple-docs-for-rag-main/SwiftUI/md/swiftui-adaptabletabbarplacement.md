

- SwiftUI
-  AdaptableTabBarPlacement 

Structure

# AdaptableTabBarPlacement

A placement for tabs in a tab view using the adaptable sidebar style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AdaptableTabBarPlacement
```

## Topics

### Type Properties

static let automatic: AdaptableTabBarPlacement

The automatic placement.

static let sidebar: AdaptableTabBarPlacement

The sidebar of a tab view.

static let tabBar: AdaptableTabBarPlacement

The tab bar of a tab view.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Configuring a tab bar

func tabViewSidebarHeader&lt;Content>(content: () -> Content) -> some View

Adds a custom header to the sidebar of a tab view.

func tabViewSidebarFooter&lt;Content>(content: () -> Content) -> some View

Adds a custom footer to the sidebar of a tab view.

func tabViewSidebarBottomBar&lt;Content>(content: () -> Content) -> some View

Adds a custom bottom bar to the sidebar of a tab view.

var tabBarPlacement: TabBarPlacement?

The current placement of the tab bar.

struct TabBarPlacement

A placement for tabs in a tab view.

var isTabBarShowingSections: Bool

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

