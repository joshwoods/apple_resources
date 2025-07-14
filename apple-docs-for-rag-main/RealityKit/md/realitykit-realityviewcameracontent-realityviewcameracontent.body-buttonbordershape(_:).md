

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  buttonBorderShape(\_:) 

Instance Method

# buttonBorderShape(\_:)

Sets the border shape for buttons in this view.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func buttonBorderShape(_ shape: ButtonBorderShape) -> some View
```

## Parameters 

`shape`  

The shape to use.

## Discussion

The border shape is used to draw the platter for a bordered button. In macOS, some border shapes are only applicable to bordered buttons in widgets.

The border shape affects buttons of the `PrimitiveButtonStyle/bordered` and `PrimitiveButtonStyle/borderedProminent` styles.

