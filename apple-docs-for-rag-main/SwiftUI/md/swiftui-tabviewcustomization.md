

- SwiftUI
-  TabViewCustomization 

Structure

# TabViewCustomization

The customizations a person makes to an adaptable sidebar tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct TabViewCustomization
```

## Overview

By default, if a person hasn’t made customizations, tabs appear according to the default builder visibilities and sections appear in the order you declare in the tab view’s tab builder.

You can change the default visibility by using the defaultVisibility(_:for:) with a sidebar placement.

You can change the default section order by changing the order in the builder. If there’s an existing persisted customization, reset the order by calling resetTabOrder() when you change the order.

All tabs and tab sections that support customization need to have a customization ID. You can mark a tab as being non-customizable by specifying a disabled behavior in all adaptable tab bar placements using customizationBehavior(_:for:).

On macOS, a default interaction is provided for reordering sections but not for controlling the visibility of individual tabs. A custom experience should be provided if desired by setting the visibility of the tab on the customization.

The following code example uses `@AppStorage` to automatically persist any visibility or section order customizations a person makes.

```
@AppStorage
private var customization: TabViewCustomization

TabView {
    Tab("Home", systemImage: "house") {
        MyHomeView()
    }
    .customizationID("com.myApp.home")

    Tab("Reports", systemImage: "chart.bar") {
        MyReportsView()
    }
    .customizationID("com.myApp.reports")

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
    .customizationID("com.myApp.browse")
}
.tabViewStyle(.sidebarAdaptable)
.tabViewCustomization($customization)
```

## Topics

### Structures

struct SectionCustomization

The customizations a user has made to a TabSection.

struct TabCustomization

The customizations a user has made to a Tab.

### Initializers

init()

Creates an empty tab sidebar customization.

### Instance Methods

func resetSectionOrder()

Resets ordering back to the default for all sections, preserving the customized tab visibilities.

func resetSectionOrder(for: String)

Resets ordering back to the default for the section with `sectionID`, preserving any customized tab visibilities.

Deprecated

func resetVisibility()

Resets all tab sidebar visibilities back to the default, preserving the section customizations.

### Subscripts

subscript(section _: String) -> TabViewCustomization.SectionCustomization

The customization of the section, identified by its customization identifier.

subscript(sectionID _: String) -> [String]?

The customization for a section’s children, identified by the section’s customization identifier.

Deprecated

subscript(sidebarVisibility _: String) -> Visibility

The visibility of the tab identified by its customization identifier.

Deprecated

subscript(tab _: String) -> TabViewCustomization.TabCustomization

The customization of the tab, identified by its customization identifier.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Enabling tab customization

func tabViewCustomization(Binding&lt;TabViewCustomization>?) -> some View

Specifies the customizations to apply to the sidebar representation of the tab view.

struct TabCustomizationBehavior

The customization behavior of customizable tab view content.

