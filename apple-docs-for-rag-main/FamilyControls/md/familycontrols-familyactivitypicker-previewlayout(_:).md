

- FamilyControls
- FamilyActivityPicker
-  previewLayout(\_:) 

Instance Method

# previewLayout(\_:)

Overrides the size of the container for the preview.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func previewLayout(_ value: PreviewLayout) -> some View
```

## Parameters 

`value`  

A layout to use for preview.

## Return Value

A preview that uses the given layout.

## Discussion

By default, previews use the `PreviewLayout/device` layout, which places the view inside a visual representation of the chosen device. You can instead tell a preview to use a different layout by choosing one of the `PreviewLayout` values, like `PreviewLayout/sizeThatFits`:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewLayout(.sizeThatFits)
    }
}
```

## See Also

### Configuring View Previews

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

func previewInterfaceOrientation(InterfaceOrientation) -> some View

Overrides the orientation of the preview.

func previewContext&lt;C>(C) -> some View

Declares a context for the preview.

