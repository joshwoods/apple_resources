

- CarPlay
-  CPMessageListItemTrailingConfiguration 

Class

# CPMessageListItemTrailingConfiguration

An object that describes the appearance of a message list item’s trailing region.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPMessageListItemTrailingConfiguration
```

## Overview

Use a trailing configuration to describe the visual elements that a message list item’s trailing region contains. The region can show a CPMessageTrailingItem and an image.

Configurations are immutable. To modify the list item’s trailing configuration, update its trailingConfiguration property with a new configuration. CarPlay detects the change and redraws the message list item.

## Topics

### Creating a Configuration

init(trailingItem: CPMessageTrailingItem, trailingImage: UIImage?)

Creates a trailing configuration that contains an item and an image.

let CPMaximumMessageItemImageSize: CGSize

The maximum size of a message list item’s image.

### Getting the Trailing Item

var trailingItem: CPMessageTrailingItem

The configuration’s item.

enum CPMessageTrailingItem

The accessories that a message list item can display in its trailing region.

### Getting the Trailing Image

var trailingImage: UIImage?

The configuration’s image.

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

class CPMessageListItemLeadingConfiguration

An object that describes the appearance of a message list item’s leading region.

var trailingConfiguration: CPMessageListItemTrailingConfiguration?

The configuration of the list item’s trailing region.

