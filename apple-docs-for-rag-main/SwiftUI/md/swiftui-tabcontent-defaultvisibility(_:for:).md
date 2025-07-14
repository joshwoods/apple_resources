

- SwiftUI
- TabContent
-  defaultVisibility(\_:for:) 

Instance Method

# defaultVisibility(\_:for:)

Configures the default visibility of a tab in customizable contexts.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func defaultVisibility(
    _ visibility: Visibility,
    for placements: AdaptableTabBarPlacement...
) -> some TabContent
```

## Parameters 

`visibility`  

The tab’s visibility.

`placements`  

The locations to apply the visibility.

## Discussion

The sidebarAdaptable style supports customization of the tab bar and sidebar on iPad. To enable customization, attach a TabViewCustomization to the TabView using tabViewCustomization(_:).

This modifier has no effect on other platforms or on a TabViewStyle that doesn’t support customization.

Note

Tabs in the sidebar represent all of the of tabs in TabView. A tab that’s hidden from the sidebar is also hidden from the top bar.

The following example shows a `TabView` with three tabs, one of which is hidden by default in the sidebar.

```
@AppStorage("MyAppTabViewCustomization")
private var customization: TabViewCustomization

TabView(selection: $selection) {
    Tab("Home", systemImage: "house", value: MyTab.home) {
        MyHomeView()
    }
    .customizationID("com.myApp.home")

    Tab("Reports", systemImage: "chart.bar", value: MyTab.reports) {
        MyReportsView()
    }
    .customizationID("com.myApp.reports")

    Tab("Browse", systemImage: "list.bullet", value: MyTab.browse) {
        MyBrowseView()
    }
    .customizationID("com.myApp.browse")
    .defaultVisibility(.hidden, for: .sidebar)
}
.tabViewStyle(.sidebarAdaptable)
.tabViewCustomization($customization)
```

