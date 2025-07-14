

- SwiftUI
- View
-  previewInterfaceOrientation(\_:) 

Instance Method

# previewInterfaceOrientation(\_:)

Overrides the orientation of the preview.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

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

By default, device previews appear right side up, using orientation portrait. You can change the orientation of a preview using one of the values in the InterfaceOrientation structure:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewInterfaceOrientation(.landscapeRight)
    }
}
```

## See Also

### Customizing a preview

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

struct PreviewDevice

A simulator device that runs a preview.

func previewLayout(PreviewLayout) -> some View

Overrides the size of the container for the preview.

struct InterfaceOrientation

The orientation of the interface from the user’s perspective.

