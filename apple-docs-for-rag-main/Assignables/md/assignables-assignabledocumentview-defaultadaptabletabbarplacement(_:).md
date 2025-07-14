

- Assignables
- AssignableDocumentView
-  defaultAdaptableTabBarPlacement(\_:) 

Instance Method

# defaultAdaptableTabBarPlacement(\_:)

Specifies the default placement for the tabs in a tab view using the adaptable sidebar style.

AssignablesSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
nonisolated
func defaultAdaptableTabBarPlacement(_ defaultPlacement: AdaptableTabBarPlacement = .automatic) -> some View
```

## Parameters 

`defaultPlacement`  

The default arrangement for the tab view.

## Discussion

This modifier is only effective on iPadOS in the `TabViewStyle/sidebarAdaptable` style. In any other configuration, the system ignores it.

The following example shows a `TabView` with three tabs, where the tab view displays the sidebar representation when the app initially launches.

```
TabView(selection: $selection) {
    Tab("Home", systemImage: "house", value: MyTab.home) {
        MyHomeView()
    }

    Tab("Downloads", systemImage: "square.and.arrow.down.fill",
        value: MyTab.downloads
    ) {
        MyDownloadsView()
    }

    Tab("Browse", systemImage: "list.bullet", value: MyTab.browse) {
        MyBrowseView()
    }
}
.tabViewStyle(.sidebarAdaptable)
.defaultAdaptableTabBarPlacement(.sidebar)
```

