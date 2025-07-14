

- UIKit
- UICollectionViewCell
-  configurationUpdateHandler 

Instance Property

# configurationUpdateHandler

A block for handling updates to the cell’s configuration using the current state.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler? { get set }
```

## Discussion

A configuration update handler provides an alternative approach to overriding updateConfiguration(using:) in a subclass. Set a configuration update handler to update the cell’s configuration using the new state in response to a configuration state change:

```
cell.configurationUpdateHandler = { cell, state in
    var content = UIListContentConfiguration.cell().updated(for: state)
    content.text = "Hello world!"
    if state.isDisabled {
        content.textProperties.color = .systemGray
    }
    cell.contentConfiguration = content
}
```

Setting the value of this property calls setNeedsUpdateConfiguration(). The system calls this handler after calling updateConfiguration(using:).

In iOS 18 and later, UIKit supports automatic trait tracking inside this closure for traits from this cell’s `traitCollection`. For more information, see Automatic trait tracking.

## See Also

### Collection view cells

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

