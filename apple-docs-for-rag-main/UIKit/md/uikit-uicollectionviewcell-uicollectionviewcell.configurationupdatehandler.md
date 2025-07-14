

- UIKit
- UICollectionViewCell
-  UICollectionViewCell.ConfigurationUpdateHandler 

Type Alias

# UICollectionViewCell.ConfigurationUpdateHandler

The type of block for handling updates to the cell’s configuration using the current state.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
typealias ConfigurationUpdateHandler = (UICollectionViewCell, UICellConfigurationState) -> Void
```

## Parameters 

`cell`  

The collection view cell to configure.

`state`  

The new state to use for updating the cell’s configuration.

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

var isSelected: Bool

The selection state of the cell.

var isHighlighted: Bool

The highlight state of the cell.

