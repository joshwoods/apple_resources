

- FamilyControls
- FamilyActivityPicker
-  navigationViewStyle(\_:) 

Instance Method

# navigationViewStyle(\_:)

Sets the style for navigation views within this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 7.0–11.4Deprecated

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

## See Also

### Styles

func buttonStyle&lt;S>(S) -> some View

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

func buttonStyle&lt;S>(S) -> some View

Sets the style for buttons within this view to a button style with a custom appearance and custom interaction behavior.

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

func menuStyle&lt;S>(S) -> some View

Sets the style for menus within this view.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

