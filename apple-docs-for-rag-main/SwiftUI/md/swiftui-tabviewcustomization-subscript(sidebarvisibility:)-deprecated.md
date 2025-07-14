

- SwiftUI
- TabViewCustomization
-  subscript(sidebarVisibility:) Deprecated

Instance Subscript

# subscript(sidebarVisibility:)

The visibility of the tab identified by its customization identifier.

iOS 18.0–18.4DeprecatediPadOS 18.0–18.4DeprecatedMac Catalyst 18.0–18.4DeprecatedmacOS 15.0–15.4DeprecatedvisionOS 2.0–2.4Deprecated

``` source
subscript(sidebarVisibility id: String) -> Visibility { get set }
```

Deprecated

Use the \`tab\` subscript and read \`sidebarVisibility\` instead.

## Overview

Visibility can be set imperatively by subscripting with the tab’s id:

```
customization[sidebarVisibility: "com.myApp.alerts"] = .hidden
```

You can change the default visibility by using the defaultVisibility(_:for:) with a sidebar placement.

```
Tab("Alerts", systemImage: "bell", value: .alerts) {
    AlertsView()
}
.customizationID("com.myApp.alerts")
.defaultVisibility(.hidden, for: .sidebar)
```

If the ID isn’t associated with a tab or the tab has not been customized, a default value of `.automatic` is returned.

