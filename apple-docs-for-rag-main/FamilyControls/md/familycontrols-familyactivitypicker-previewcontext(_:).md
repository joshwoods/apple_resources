

- FamilyControls
- FamilyActivityPicker
-  previewContext(\_:) 

Instance Method

# previewContext(\_:)

Declares a context for the preview.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func previewContext(_ value: C) -> some View where C : PreviewContext
```

## Parameters 

`value`  

The context for the preview; the default is `nil`.

## See Also

### Configuring View Previews

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

func previewLayout(PreviewLayout) -> some View

Overrides the size of the container for the preview.

func previewInterfaceOrientation(InterfaceOrientation) -> some View

Overrides the orientation of the preview.

