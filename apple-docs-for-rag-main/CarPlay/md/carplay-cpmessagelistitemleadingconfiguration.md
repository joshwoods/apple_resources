

- CarPlay
-  CPMessageListItemLeadingConfiguration 

Class

# CPMessageListItemLeadingConfiguration

An object that describes the appearance of a message list item’s leading region.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPMessageListItemLeadingConfiguration
```

## Overview

Use a leading configuration to describe the visual elements that a message list item’s leading region contains. The region can show a CPMessageLeadingItem, an image, and an unread indicator.

Configurations are immutable. To modify the list item’s leading configuration, update its leadingConfiguration property with a new configuration. CarPlay detects the change and redraws the message list item.

## Topics

### Creating a Configuration

init(leadingItem: CPMessageLeadingItem, leadingImage: UIImage?, unread: Bool)

Creates a leading configuration that contains an item and an image.

let CPMaximumMessageItemImageSize: CGSize

The maximum size of a message list item’s image.

### Getting the Leading Item

var leadingItem: CPMessageLeadingItem

The configuration’s item.

enum CPMessageLeadingItem

The accessories that a message list item can display in its leading region.

### Getting the Configuration’s State

var leadingImage: UIImage?

The configuration’s image.

var isUnread: Bool

A Boolean value that determines whether the message list item displays an unread indicator.

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

## See Also

### Managing Leading and Trailing Configurations

var leadingConfiguration: CPMessageListItemLeadingConfiguration

The configuration of the list item’s leading region.

var trailingConfiguration: CPMessageListItemTrailingConfiguration?

The configuration of the list item’s trailing region.

class CPMessageListItemTrailingConfiguration

An object that describes the appearance of a message list item’s trailing region.

