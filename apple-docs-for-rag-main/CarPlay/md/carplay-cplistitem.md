

- CarPlay
-  CPListItem 

Class

# CPListItem

A selectable row in a list template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPListItem
```

## Overview

A list item manages the content of a single row in a list template. CarPlay manages the layout of a list item and may adjust its layout to allow for the display of auxiliary content, such as an accessory or a Now Playing indicator. A list item can display primary and secondary text and an image. It can also show an accessory or custom accessory image, and one of several indicators that the system provides.

You assign a handler to a list item that CarPlay executes when the user selects the item. The handler receives the item and a closure that you must call after you finish processing the selection.

CarPlay doesn’t support custom list item types. Instead, use the userInfo property to attach a value to the list item that provides additional context, such as specifying a model object that corresponds to the item.

## Topics

### Creating a List Item

init(text: String?, detailText: String?)

Creates a list item with primary and secondary text.

init(text: String?, detailText: String?, image: UIImage?)

Creates a list item with primary text, secondary text, and an image.

init(text: String?, detailText: String?, image: UIImage?, accessoryImage: UIImage?, accessoryType: CPListItemAccessoryType)

Creates a list item that displays an accessory beside its content.

### Managing Configuration

var isEnabled: Bool

A Boolean value that indicates if the item is enabled.

var handler: ((any CPSelectableListItem, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects the list item.

var userInfo: Any?

An opaque value for the list item.

### Managing Accessories

var accessoryType: CPListItemAccessoryType

The accessory that the list item displays in its trailing region.

enum CPListItemAccessoryType

The accessory types that a list item can display.

var accessoryImage: UIImage?

The image that the list item displays in its trailing region.

func setAccessoryImage(UIImage?)

Updates the list item’s accessory image.

### Managing Content

var text: String?

The list item’s primary text.

func setText(String)

Updates the list item’s primary text.

var detailText: String?

The list item’s secondary text.

func setDetailText(String?)

Updates the list item’s secondary text.

var image: UIImage?

The image that the list item displays in its leading region.

func setImage(UIImage?)

Updates the list item’s image.

class var maximumImageSize: CGSize

The maximum size of a list item’s image and accessory image.

### Managing Playback Information

var isExplicitContent: Bool

A Boolean value that determines whether the list item displays its explicit content indicator.

var isPlaying: Bool

A Boolean value that determines whether the list item displays its Now Playing indicator.

var playingIndicatorLocation: CPListItemPlayingIndicatorLocation

The location where the list item displays its Now Playing indicator.

enum CPListItemPlayingIndicatorLocation

The locations where a list item can display the Now Playing indicator.

var playbackProgress: CGFloat

The playback progress status for the content that the list item represents.

### Managing the Assistant Cell

enum AssistantCellPosition

Constants to specify the position of the assistant cell.

enum AssistantCellVisibility

Constants to specify the visibility of the assistant cell.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CPListTemplateItem
- CPSelectableListItem
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating a Section

init(items: [any CPListTemplateItem], header: String, headerSubtitle: String?, headerImage: UIImage?, headerButton: CPButton?, sectionIndexTitle: String?)

Creates a section with list items, a header, a section index title, and section header details.

protocol CPListTemplateItem

A description of the common properties of all list item types.

protocol CPSelectableListItem

A description of a selectable list item.

class CPListImageRowItem

A list template row that displays a series of images.

class CPMessageListItem

A list template row that represents a conversation or contact.

