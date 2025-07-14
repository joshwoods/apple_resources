

- RealityKit
- RealityViewAttachmentBuilderContent
-  tabViewSidebarBottomBar(content:) 

Instance Method

# tabViewSidebarBottomBar(content:)

Adds a custom bottom bar to the sidebar of a tab view.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

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

