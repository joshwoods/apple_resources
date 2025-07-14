

- UIKit
- UICellAccessory
- UICellAccessory.Placement
-  UICellAccessory.Placement.Position 

Type Alias

# UICellAccessory.Placement.Position

The index position of the cell accessory in relation to the other accessories in the specified array.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
typealias Position = ([UICellAccessory]) -> Int
```

## See Also

### Specifying position

static func position(after: UICellAccessory) -> UICellAccessory.Placement.Position

Provides a position after the accessory that matches the specified type, or at the end if there’s no matching type.

static func position(before: UICellAccessory) -> UICellAccessory.Placement.Position

Provides a position before the accessory that matches the specified type, or at the beginning if there’s no matching type.

