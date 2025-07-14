

- UIKit
-  UIContextMenuConfiguration 

Class

# UIContextMenuConfiguration

An object containing the configuration details for the contextual menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UIContextMenuConfiguration
```

## Overview

Before displaying a contextual menu, the system asks your UIContextMenuInteractionDelegate to provide a UIContextMenuConfiguration object with details about that menu. In your contextMenuInteraction(_:configurationForMenuAtLocation:) method, use the location parameter to determine where the interaction occurred, and use the content at that location to configure your contextual menu and view controller. Provide custom blocks to generate:

- The contextual menu with the actions for your content.

- An optional view controller to use when displaying your content.

If you specify a default object without any custom handler blocks, the system displays a default preview interface with no menu.

## Topics

### Creating the menu configuration object

convenience init(identifier: (any NSCopying)?, previewProvider: UIContextMenuContentPreviewProvider?, actionProvider: UIContextMenuActionProvider?)

Creates a menu configuration object with the specified action and preview providers.

typealias UIContextMenuContentPreviewProvider

Returns the custom view controller to use when previewing your content.

typealias UIContextMenuActionProvider

Returns an action-based contextual menu, optionally incorporating the system-suggested actions.

### Getting the configuration identifier

var identifier: any NSCopying

The unique identifier for this configuration object.

### Handling multiple-item interactions

var secondaryItemIdentifiers: Set&lt;AnyHashable>

A set of identifiers corresponding to each item other than the primary item in a multiple-item interaction.

var badgeCount: Int

The number of items in a multiple-item interaction.

### Specifying the order of menu elements

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

enum ElementOrder

Constants that define the ordering strategy for menu elements in a context menu.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Providing the preview configuration data

func contextMenuInteraction(UIContextMenuInteraction, configurationForMenuAtLocation: CGPoint) -> UIContextMenuConfiguration?

Returns the configuration data to use when previewing the content.

**Required**

