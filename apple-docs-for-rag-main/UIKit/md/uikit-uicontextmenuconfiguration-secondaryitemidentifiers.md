

- UIKit
- UIContextMenuConfiguration
-  secondaryItemIdentifiers 

Instance Property

# secondaryItemIdentifiers

A set of identifiers corresponding to each item other than the primary item in a multiple-item interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var secondaryItemIdentifiers: Set { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

When the context menu acts on multiple items, you can use this property to include the identifiers of the secondary items in the configuration. You don’t need to set this property when you create a configuration that originates from a multiple-item interaction in a collection view, such as in collectionView(_:contextMenuConfigurationForItemsAt:point:).

## See Also

### Handling multiple-item interactions

var badgeCount: Int

The number of items in a multiple-item interaction.

