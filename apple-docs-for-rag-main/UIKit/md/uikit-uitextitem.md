

- UIKit
-  UITextItem 

Class

# UITextItem

An object for attaching custom actions and menus to links, text attachments, or other specific text in a text view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
class UITextItem
```

## Overview

A text item represents a link with a URL destination, a custom tag for a topic that you specify in your app, or a text attachment in a text view. In your text view’s UITextViewDelegate, implement textView(_:primaryActionFor:defaultAction:) to provide a custom action when someone interacts with a text item. Implement textView(_:menuConfigurationFor:defaultMenu:) to provide a custom menu for a text item.

## Topics

### Specifying the content type

var content: UITextItem.Content

The content type and related value of the text item.

enum Content

Constants that describe and capture the type of content a text item represents along with a specific related value.

### Specifying the range

var range: NSRange

The range that delineates the text item in an attributed string.

### Creating a menu

class MenuConfiguration

An object that describes what type of menu and preview to show for a text item.

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

class MenuConfiguration

An object that describes what type of menu and preview to show for a text item.

protocol UITextViewDelegate

The methods for receiving editing-related messages for text view objects.

