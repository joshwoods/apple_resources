

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  navigationBarTitle(\_:) 

Instance Method

# navigationBarTitle(\_:)

Sets the title of this view’s navigation bar with a localized string.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac CatalysttvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func navigationBarTitle(_ titleKey: LocalizedStringKey) -> some View
```

## Parameters 

`titleKey`  

A key to a localized description of this view to display in the navigation bar.

## Discussion

Use `navigationBarTitle(_:)` to set the title of the navigation bar using a `LocalizedStringKey` that will be used to search for a matching localized string in the application’s localizable strings assets.

This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

In the example below, a string constant is used to access a `LocalizedStringKey` that will be resolved at run time to provide a title for the navigation bar. If the localization key cannot be resolved, the text of the key name will be used as the title text.

```
struct FlavorView: View {
    let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                 "Pistachio"]
    var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle("Today's Flavors")
        }
    }
}
```

