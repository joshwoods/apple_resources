

- UIKit
- UICellAccessory
- UICellAccessory.Placement
-  UICellAccessory.Placement.leading(displayed:at:) 

Case

# UICellAccessory.Placement.leading(displayed:at:)

The accessory appears on the leading edge of the cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case leading(
    displayed: UICellAccessory.DisplayedState = .always,
    at: UICellAccessory.Placement.Position = { $0.count }
)
```

## See Also

### Specifying accessory placement

case trailing(displayed: UICellAccessory.DisplayedState, at: UICellAccessory.Placement.Position)

The accessory appears on the trailing edge of the cell.

