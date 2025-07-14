

- FamilyControls
- FamilyActivityPicker
-  progressViewStyle(\_:) 

Instance Method

# progressViewStyle(\_:)

Sets the style for progress views in this view.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func progressViewStyle(_ style: S) -> some View where S : ProgressViewStyle
```

## Parameters 

`style`  

The progress view style to use for this view.

## Discussion

For example, the following code creates a progress view that uses the “circular” style:

```
ProgressView()
    .progressViewStyle(.circular)
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

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

