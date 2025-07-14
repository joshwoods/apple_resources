

- SwiftUI
- TabContent
-  disabled(\_:) 

Instance Method

# disabled(\_:)

Controls whether users can interact with this tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+

``` source
nonisolated
func disabled(_ disabled: Bool) -> some TabContent
```

## Parameters 

`disabled`  

A Boolean value that determines whether users can interact with this tab.

## Discussion

The following example shows a TabView with one tab that is not selectable.

```
TabView {
    Tab("Home", systemImage: "house") {
        HomeView()
    }
    Tab("Alerts", systemImage: "bell") {
        AlertsView()
    }
    .disabled(alertsDisabled)
}
```

