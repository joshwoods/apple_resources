

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  previewLayout(\_:) 

Instance Method

# previewLayout(\_:)

Overrides the size of the container for the preview.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+watchOS 6.0+

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

