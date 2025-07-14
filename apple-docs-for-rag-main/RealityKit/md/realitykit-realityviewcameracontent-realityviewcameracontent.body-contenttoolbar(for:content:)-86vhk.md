

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  contentToolbar(for:content:) 

Instance Method

# contentToolbar(for:content:)

Populates the toolbar of the specified content view type with the views you provide.

RealityKitSwiftUIiOS 18.4+iPadOS 18.4+Mac CatalystmacOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
nonisolated
func contentToolbar(
    for placement: ContentToolbarPlacement,
    @ViewBuilder content: () -> Content
) -> some View where Content : View
```

## Parameters 

`content`  

The views representing the content of the toolbar.

## Discussion

Use this modifier to add toolbar content that remains consistent regardless of the content view.

Unlike the toolbar modifier, which configures the toolbar of the modified view’s container, the `contentToolbar` modifier configures the toolbar within the modified view’s content instead. This means that the `contentToolbar` modifier should generally be applied directly to a container view, instead of to the content within a container view. For example, to configure the toolbar of tab view’s sidebar, apply the `contentToolbar` modifier to the `TabView` itself, not to any of the tabs within the `TabView`.

The example below adds a button to the tab view sidebar.

```
TabView {
    Tab("Home", systemImage: "house") {
        HomeView()
    }

    Tab("Alerts", systemImage: "bell") {
        AlertsView()
    }

    TabSection("Categories") {
        Tab("Climate", systemImage: "fan") {
            ClimateView()
        }

        Tab("Lights", systemImage: "lightbulb") {
            LightsView()
        }
    }
}
.tabViewStyle(.sidebarAdaptable)
.contentToolbar(for: .tabViewSidebar) {
    DisconnectDevicesButton()
}
```

