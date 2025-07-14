

- SwiftUI
- View
-  tabViewSidebarHeader(content:) 

Instance Method

# tabViewSidebarHeader(content:)

Adds a custom header to the sidebar of a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func tabViewSidebarHeader(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Discussion

The header appears at the top of the sidebar before any tab labels and can scroll with the content. The header is only visible when the TabView is displaying the sidebar.

The following example adds a welcome message to the top of the sidebar:

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
.tabViewSidebarHeader {
    WelcomeHeaderView()
}
```

Note

To have a sidebar, aTabView needs the sidebarAdaptable style.

## See Also

### Configuring a tab bar

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

var isTabBarShowingSections: Bool

A Boolean value that determines whether a tab view shows the expanded contents of a tab section.

