

- RealityKit
- Model3DPlaceholderContent
-  navigationViewStyle(\_:) 

Instance Method

# navigationViewStyle(\_:)

Sets the style for navigation views within this view.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 7.0+

``` source
nonisolated
func navigationViewStyle(_ style: S) -> some View where S : NavigationViewStyle
```

## Discussion

Use this modifier to change the appearance and behavior of navigation views. For example, by default, navigation views appear with multiple columns in wider environments, like iPad in landscape orientation:

You can apply the `NavigationViewStyle/stack` style to force single-column stack navigation in these environments:

```
NavigationView {
    List {
        NavigationLink("Purple", destination: ColorDetail(color: .purple))
        NavigationLink("Pink", destination: ColorDetail(color: .pink))
        NavigationLink("Orange", destination: ColorDetail(color: .orange))
    }
    .navigationTitle("Colors")

    Text("Select a Color") // A placeholder to show before selection.
}
.navigationViewStyle(.stack)
```

