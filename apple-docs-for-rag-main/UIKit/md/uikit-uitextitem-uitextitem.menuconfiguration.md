

- UIKit
- UITextItem
-  UITextItem.MenuConfiguration 

Class

# UITextItem.MenuConfiguration

An object that describes what type of menu and preview to show for a text item.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
class MenuConfiguration
```

## Overview

Create and return a menu configuration for a text item in textView(_:menuConfigurationFor:defaultMenu:) to provide a custom menu that the system shows when someone interacts with the text item. Provide a custom view for the item’s preview, or specify that the system displays a default preview.

## Topics

### Creating a menu configuration

convenience init(preview: UITextItem.MenuConfiguration.Preview?, menu: UIMenu)

Creates a text item menu configuration with the specified menu and preview.

enum Preview

Constants that indicate what type of preview to display alongside the text item’s menu.

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

### Text actions and menus

class UITextItem

An object for attaching custom actions and menus to links, text attachments, or other specific text in a text view.

protocol UITextViewDelegate

The methods for receiving editing-related messages for text view objects.

