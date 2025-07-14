

- SwiftUI
- TabContent
-  badge(\_:) 

Instance Method

# badge(\_:)

Generates a badge for a tab from an integer value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func badge(_ count: Int) -> some TabContent
```

Show all declarations

## Parameters 

`count`  

An integer value to display in the badge. Set the value to zero to hide the badge.

## Discussion

Use a badge to convey optional, supplementary information about a view. The number provided will appear as a numerical indicator on the given tab.

The following example shows a TabView with the value of `alerts.count` displayed as a badge on the alerts tab.

```
TabView {
    Tab("Home", systemImage: "house") {
        HomeView()
    }
    Tab("Alerts", systemImage: "bell") {
        AlertsView()
    }
    .badge(alerts.count)
}
```

