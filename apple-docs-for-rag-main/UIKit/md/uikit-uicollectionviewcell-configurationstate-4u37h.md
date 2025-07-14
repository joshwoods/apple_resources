

- UIKit
- UICollectionViewCell
-  configurationState 

Instance Property

# configurationState

The current configuration state of the cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @objc(_bridgedConfigurationState) @preconcurrency
dynamic var configurationState: UICellConfigurationState { get }
```

## Discussion

To add your own custom state, see UIConfigurationStateCustomKey.

## See Also

### Managing the state

func setNeedsUpdateConfiguration()

Informs the cell to update its configuration for its current state.

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the cell’s configuration using the current state.

var isSelected: Bool

The selection state of the cell.

var isHighlighted: Bool

The highlight state of the cell.

