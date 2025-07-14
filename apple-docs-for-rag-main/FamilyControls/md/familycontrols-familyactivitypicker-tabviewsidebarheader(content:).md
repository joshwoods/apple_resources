

- FamilyControls
- FamilyActivityPicker
-  tabViewSidebarHeader(content:) 

Instance Method

# tabViewSidebarHeader(content:)

Adds a custom header to the sidebar of a tab view.

FamilyControlsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func tabViewSidebarHeader(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Discussion

The header appears at the top of the sidebar before any tab labels and can scroll with the content. The header is only visible when the `TabView` is displaying the sidebar.

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

To have a sidebar, a`TabView` needs the `TabViewStyle/sidebarAdaptable` style.

