

- FamilyControls
- FamilyActivityPicker
-  previewInterfaceOrientation(\_:) 

Instance Method

# previewInterfaceOrientation(\_:)

Overrides the orientation of the preview.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func previewInterfaceOrientation(_ value: InterfaceOrientation) -> some View
```

## Parameters 

`value`  

An orientation to use for preview.

## Return Value

A preview that uses the given orientation.

## Discussion

By default, device previews appear right side up, using orientation `InterfaceOrientation/portrait`. You can change the orientation of a preview using one of the values in the `InterfaceOrientation` structure:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewInterfaceOrientation(.landscapeRight)
    }
}
```

## See Also

### Configuring View Previews

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

func previewLayout(PreviewLayout) -> some View

Overrides the size of the container for the preview.

func previewContext&lt;C>(C) -> some View

Declares a context for the preview.

