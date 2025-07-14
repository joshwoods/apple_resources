

- SwiftUI
- PointerStyle
-  image(\_:hotSpot:) 

Type Method

# image(\_:hotSpot:)

Initializes a pointer style with a given image and hot spot.

macOS 15.0+

``` source
static func image(
    _ image: Image,
    hotSpot: UnitPoint
) -> PointerStyle
```

Show all declarations

## Parameters 

`image`  

The pointer image.

`hotSpot`  

The point on the image that represents the location from which the pointer interaction occurs. For example, the hot spot of an arrow-shaped pointer is the tip of the arrow.

## Discussion

The hot spot is the part of the pointer that must be positioned over an onscreen element for clicking to have an effect.

For guidance on using a custom pointer, refer to Pointing devices in the Human Interface Guidelines.

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

