

- UIKit
- UICellAccessory
-  UICellAccessory.Placement 

Enumeration

# UICellAccessory.Placement

Constants that describe the placement of the accessory within the cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
enum Placement
```

## Topics

### Specifying accessory placement

case leading(displayed: UICellAccessory.DisplayedState, at: UICellAccessory.Placement.Position)

The accessory appears on the leading edge of the cell.

case trailing(displayed: UICellAccessory.DisplayedState, at: UICellAccessory.Placement.Position)

The accessory appears on the trailing edge of the cell.

### Specifying position

static func position(after: UICellAccessory) -> UICellAccessory.Placement.Position

Provides a position after the accessory that matches the specified type, or at the end if there’s no matching type.

static func position(before: UICellAccessory) -> UICellAccessory.Placement.Position

Provides a position before the accessory that matches the specified type, or at the beginning if there’s no matching type.

typealias Position

The index position of the cell accessory in relation to the other accessories in the specified array.

## See Also

### Customizing appearance and placement

enum LayoutDimension

Constants that describe the layout dimension for the accessory.

enum DisplayedState

Constants that describe the cell-editing states that the accessory appears in.

