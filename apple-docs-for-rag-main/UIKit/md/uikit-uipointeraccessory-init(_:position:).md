

- UIKit
- UIPointerAccessory
-  init(\_:position:) 

Initializer

# init(\_:position:)

Creates a pointer accessory with the specified shape and position.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(
    _ shape: UIPointerShape,
    position: UIPointerAccessory.Position
)
```

## Parameters 

`shape`  

One of the available UIPointerShape shapes.

`position`  

One of the available UIPointerAccessory.Position positions.

## See Also

### Creating a pointer accessory

class func arrow(UIPointerAccessory.Position) -> Self

Creates a pointer accessory with an arrow shape at the specified position.

