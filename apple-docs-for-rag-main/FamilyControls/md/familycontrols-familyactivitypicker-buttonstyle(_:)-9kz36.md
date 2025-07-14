

- FamilyControls
- FamilyActivityPicker
-  buttonStyle(\_:) 

Instance Method

# buttonStyle(\_:)

Sets the style for buttons within this view to a button style with a custom appearance and custom interaction behavior.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func buttonStyle(_ style: S) -> some View where S : PrimitiveButtonStyle
```

## Discussion

Use this modifier to set a specific style for button instances within a view:

```
HStack {
    Button("Sign In", action: signIn)
    Button("Register", action: register)
}
.buttonStyle(.bordered)
```

## See Also

### Styles

func buttonStyle&lt;S>(S) -> some View

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

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

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

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

