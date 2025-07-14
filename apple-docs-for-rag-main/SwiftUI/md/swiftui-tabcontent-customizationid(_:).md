

- SwiftUI
- TabContent
-  customizationID(\_:) 

Instance Method

# customizationID(\_:)

Sets the identifier for a tab to persist its state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func customizationID(_ id: String) -> some TabContent
```

## Parameters 

`id`  

The identifier to associate with a tab or section.

## Discussion

The identifier needs to be stable, including across app version updates.

Only the sidebarAdaptable style supports supports customization. To enable customization, attach a TabViewCustomization to the TabView using tabViewCustomization(_:).

All tabs and tab sections that support customization are required to have a customization ID. You can mark a tab as being non-customizable by specifying a disabled behavior in all adaptable tab bar placements using customizationBehavior(_:for:).

If you apply a customization ID to a TabSection, ensure you specify customization IDs for all of the tabs within the section, unless the tab has been marked as having customization turned off.

The following example adds customization identifiers to all tabs and tab sections.

```
@AppStorage("MyAppTabViewCustomization")
private var customization: TabViewCustomization

TabView {
    Tab("Home", systemImage: "house") {
        HomeView()
    }
    .customizationID("com.myApp.home")

    Tab("Alerts", systemImage: "bell") {
        AlertsView()
    }
    .customizationID("com.myApp.bell")

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
}
.tabViewStyle(.sidebarAdaptable)
.tabViewCustomization($customization)
```

