

- UIKit
- UICellAccessory
- UICellAccessory.Placement
-  position(before:) 

Type Method

# position(before:)

Provides a position before the accessory that matches the specified type, or at the beginning if there’s no matching type.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func position(before accessory: UICellAccessory) -> UICellAccessory.Placement.Position
```

## See Also

### Specifying position

static func position(after: UICellAccessory) -> UICellAccessory.Placement.Position

Provides a position after the accessory that matches the specified type, or at the end if there’s no matching type.

typealias Position

The index position of the cell accessory in relation to the other accessories in the specified array.

