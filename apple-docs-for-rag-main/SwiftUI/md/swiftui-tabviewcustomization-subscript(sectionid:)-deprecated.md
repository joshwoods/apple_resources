

- SwiftUI
- TabViewCustomization
-  subscript(sectionID:) Deprecated

Instance Subscript

# subscript(sectionID:)

The customization for a section’s children, identified by the section’s customization identifier.

iOS 18.0–18.4DeprecatediPadOS 18.0–18.4DeprecatedMac Catalyst 18.0–18.4DeprecatedmacOS 15.0–15.4DeprecatedvisionOS 2.0–2.4Deprecated

``` source
subscript(sectionID id: String) -> [String]? { get }
```

Deprecated

Use the \`section\` subscript and read \`tabOrder\` instead.

## Overview

Section order can be read by subscripting with the tab section’s id:

```
let order = customization[sectionID: "com.myApp.categories"]
```

Identifiers can be associated with a `Tab` or `TabSection` using the `customizationID(_:)` modifier.

```
TabSection("Categories") {
    Tab("Climate", systemImage: "fan") {
        ClimateView()
    }
    .customizationID("com.myApp.climate")

    Tab("Lights", systemImage: "lightbulb") {
        LightsView()
    }
    .customizationID("com.myApp.lights")
}
.customizationID("com.myApp.categories")
```

If the ID isn’t associated with a section or the section has not been customized, a default value of `nil` is returned.

