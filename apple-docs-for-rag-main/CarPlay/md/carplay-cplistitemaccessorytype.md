

- CarPlay
-  CPListItemAccessoryType 

Enumeration

# CPListItemAccessoryType

The accessory types that a list item can display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum CPListItemAccessoryType
```

## Overview

Use these constants to set the value of a list item’s accessoryType property. An accessory can provide additional context for a list item’s contents, or help communicate its behavior.

## Topics

### Accessory Types

case none

Don’t show an accessory.

case disclosureIndicator

Show a chevron icon.

case cloud

Show a cloud icon.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Accessories

var accessoryType: CPListItemAccessoryType

The accessory that the list item displays in its trailing region.

var accessoryImage: UIImage?

The image that the list item displays in its trailing region.

func setAccessoryImage(UIImage?)

Updates the list item’s accessory image.

