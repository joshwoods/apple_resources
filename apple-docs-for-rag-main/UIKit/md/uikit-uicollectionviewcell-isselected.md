

- UIKit
- UICollectionViewCell
-  isSelected 

Instance Property

# isSelected

The selection state of the cell.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isSelected: Bool { get set }
```

## Discussion

This property manages the selection state of the cell only. The default value of this property is false, which indicates an unselected state.

You typically don’t set the value of this property directly. Changing the value of this property programmatically doesn’t change the appearance of the cell. The preferred way to select the cell and highlight it’s to use the selection methods of the collection view object.

## See Also

### Managing the state

var configurationState: UICellConfigurationState

The current configuration state of the cell.

func setNeedsUpdateConfiguration()

Informs the cell to update its configuration for its current state.

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the cell’s configuration using the current state.

var isHighlighted: Bool

The highlight state of the cell.

