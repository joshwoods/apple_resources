

- UIKit
- UICellAccessory
- UICellAccessory.Placement
-  UICellAccessory.Placement.trailing(displayed:at:) 

Case

# UICellAccessory.Placement.trailing(displayed:at:)

The accessory appears on the trailing edge of the cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case trailing(
    displayed: UICellAccessory.DisplayedState = .always,
    at: UICellAccessory.Placement.Position = { _ in 0 }
)
```

## See Also

### Specifying accessory placement

case leading(displayed: UICellAccessory.DisplayedState, at: UICellAccessory.Placement.Position)

The accessory appears on the leading edge of the cell.

