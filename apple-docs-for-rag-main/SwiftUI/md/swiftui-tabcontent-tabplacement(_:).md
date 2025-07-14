

- SwiftUI
- TabContent
-  tabPlacement(\_:) 

Instance Method

# tabPlacement(\_:)

Specifies the placement of a tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func tabPlacement(_ placement: TabPlacement) -> some TabContent
```

## Parameters 

`placement`  

The location of the tab.

## Discussion

The following example shows a TabView with three tabs where the second tab is pinned to the trailing edge of the top tab bar on iPad.

```
TabView {
    Tab("Home", systemImage: "house") {
        MyHomeView()
    }

    Tab("Downloads", systemImage: "square.and.arrow.down.fill") {
        MyDownloadsView()
    }
    .tabPlacement(.pinned)

    Tab("Browse", systemImage: "list.bullet") {
        MyBrowseView()
    }
}
.tabViewStyle(.sidebarAdaptable)
```

