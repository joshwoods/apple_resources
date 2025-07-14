

- UIKit
-  UIListSeparatorConfiguration 

Structure

# UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

iOS 14.5+iPadOS 14.5+Mac CatalystvisionOS

``` source
struct UIListSeparatorConfiguration
```

## Overview

To specify list separator appearance for a section, set a default sectionwide separatorConfiguration on your UICollectionLayoutListConfiguration when you create your list.

```
var listConfig = UICollectionLayoutListConfiguration(appearance: .plain)
listConfig.separatorConfiguration.color = .tertiarySystemFill
let layout = UICollectionViewCompositionalLayout.list(using: listConfig)
```

To override list separator appearance on a per-item basis, use the itemSeparatorHandler property.

```
var listConfig = UICollectionLayoutListConfiguration(appearance: .plain)
listConfig.separatorConfiguration.color = .tertiarySystemFill

let indexPathToHide = IndexPath()

listConfig.itemSeparatorHandler = { (indexPath, sectionSeparatorConfiguration) in    
    var configuration = sectionSeparatorConfiguration
    if indexPath == indexPathToHide {
        configuration.bottomSeparatorVisibility = .hidden    
    }    
    return configuration
}

let layout = UICollectionViewCompositionalLayout.list(using: listConfig)
```

## Topics

### Creating a list separator configuration

init(listAppearance: UICollectionLayoutListConfiguration.Appearance)

Creates a list separator configuration with default values according to the specified list appearance.

### Controlling separator visibility

var topSeparatorVisibility: UIListSeparatorConfiguration.Visibility

The visibility of the top separator for the item the configuration applies to.

var bottomSeparatorVisibility: UIListSeparatorConfiguration.Visibility

The visibility of the bottom separator for the item the configuration applies to.

enum Visibility

Constants that define the visibility of list separators.

### Configuring separator insets

var topSeparatorInsets: NSDirectionalEdgeInsets

Insets to apply to the top separator of the item the configuration applies to.

var bottomSeparatorInsets: NSDirectionalEdgeInsets

Insets to apply to the bottom separator of the item the configuration applies to.

static let automaticInsets: NSDirectionalEdgeInsets

A constant that specifies a placeholder size for separator insets.

### Configuring separator appearance

var color: UIColor

The color to use for the separators of the item the configuration applies to.

var multipleSelectionColor: UIColor

The color to use for the separators of the item the configuration applies to when the item is in a multiple-selection group.

var visualEffect: UIVisualEffect?

The visual effect to use for the separators of the item the configuration applies to.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Configuring separators

var showsSeparators: Bool

A Boolean value that determines whether the list shows separators between cells.

var separatorConfiguration: UIListSeparatorConfiguration

The section’s preferred configuration for list separators.

var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler?

The closure that provides granular control over the list separator appearance of each item.

typealias ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

