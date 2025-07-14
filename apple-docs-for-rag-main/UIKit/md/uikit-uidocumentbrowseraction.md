

- UIKit
-  UIDocumentBrowserAction 

Class

# UIDocumentBrowserAction

A custom action that you can create and add to a document browser’s Edit menu or navigation bar.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIDocumentBrowserAction
```

## Mentioned in 

Adding custom actions and activities

## Overview

By default, the system provides a number of standard actions (copy, move, rename, delete, and share). To add custom actions, assign an array of UIDocumentBrowserAction objects to the browser’s customActions property.

Document browser actions can appear in either the navigation bar or the Edit menu.

- *Navigation bar* actions appear in the navigation bar when the user places the browser into the Select mode.

- *Menu* actions appear in the Edit Menu when the user long presses on a document or folder.

When triggered, these actions are passed the URLs of the currently selected items.

## Topics

### Creating and configuring actions

init(identifier: String, localizedTitle: String, availability: UIDocumentBrowserAction.Availability, handler: ([URL]) -> Void)

Instantiates and returns a new browser action item.

var image: UIImage?

The action’s image displayed in the navigation bar.

var supportedContentTypes: [String]

An array of uniform type identifiers that define the types of documents that the action supports.

var supportsMultipleItems: Bool

A Boolean value that determines whether the action can be triggered on more than one document at a time.

### Accessing activity data

var identifier: String

The action’s unique identifier.

var localizedTitle: String

The title that appears in the menu or navigation bar.

var availability: UIDocumentBrowserAction.Availability

A value that defines where the action can appear (in the Edit Menu, the navigation bar, or both).

struct Availability

Values that determine where the action can appear in the document browser.

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

### Related Documentation

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

### Adding custom actions

var customActions: [UIDocumentBrowserAction]

Custom document browser actions.

