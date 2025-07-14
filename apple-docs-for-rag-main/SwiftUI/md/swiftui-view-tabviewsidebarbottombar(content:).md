

- SwiftUI
- View
-  tabViewSidebarBottomBar(content:) 

Instance Method

# tabViewSidebarBottomBar(content:)

Adds a custom bottom bar to the sidebar of a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func tabViewSidebarBottomBar(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Discussion

The content is pinned at the bottom of the sidebar, so it’s always visible when the sidebar is visible and doesn’t scroll with the content.

The following example adds an account button to the bottom of the sidebar:

```
TabView {
    Tab("Home", systemImage: "house") {
        HomeView()
    }

    Tab("Alerts", systemImage: "bell") {
        AlertsView()
    }

    Tab("Browse", systemImage: "list.bullet") {
        MyBrowseView()
    }
}
.tabViewStyle(.sidebarAdaptable)
.tabViewSidebarBottomBar {
    AccountButton()
}
```

## See Also

### Configuring a tab bar

func tabViewSidebarHeader&lt;Content>(content: () -> Content) -> some View

Adds a custom header to the sidebar of a tab view.

func tabViewSidebarFooter&lt;Content>(content: () -> Content) -> some View

Adds a custom footer to the sidebar of a tab view.

struct AdaptableTabBarPlacement

A placement for tabs in a tab view using the adaptable sidebar style.

var tabBarPlacement: TabBarPlacement?

The current placement of the tab bar.

struct TabBarPlacement

A placement for tabs in a tab view.

var isTabBarShowingSections: Bool

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

