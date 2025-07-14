

- CarPlay
-  CPListImageRowItem 

Class

# CPListImageRowItem

A list template row that displays a series of images.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPListImageRowItem
```

## Overview

Use `CPListImageRowItem` to display a series of images as a row in a list template. At runtime, use CPMaximumNumberOfGridImages to determine the maximum number of images that the row displays. CarPlay may display fewer images, depending on the width of the vehicle’s primary screen. Provide images that are display-ready, and include light and dark variants of each. See init(text:images:) for more information.

You assign a handler to the list item that CarPlay executes when the user selects the item. You can assign a second handler, listImageRowHandler, which CarPlay calls when the user selects an individual image.

CarPlay doesn’t support custom list item types. Instead, use the `userInfo` property to attach a value to the list item that provides additional context, such as specifying a model object that corresponds to the item.

## Topics

### Creating a List Image Row Item

init(text: String, images: [UIImage])

Creates a list item that displays a row of images.

init(text: String, images: [UIImage], imageTitles: [String])

Creates a list item that displays a row of images with a title below each image.

### Managing Content

var text: String?

The list item’s primary text.

var gridImages: [UIImage]

The images that appear in the list item’s image row.

func update([UIImage])

Adds, removes, reorders, or updates the images in the list item’s image row.

class var maximumImageSize: CGSize

The maximum size of an image that an image row can display.

let CPMaximumNumberOfGridImages: Int

The maximum number of images that an image row can contain.

### Managing Selection

var listImageRowHandler: ((CPListImageRowItem, Int, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects an image.

var handler: ((any CPSelectableListItem, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects the list item.

### Managing Supplementary Information

var userInfo: Any?

An opaque value for the list item.

### Enabling Items

var isEnabled: Bool

A Boolean value that indicates if the item is enabled.

### Instance Properties

var imageTitles: [String]

Update the titles displayed each image in this image row item. If this image row item is already displayed in a list template, then it will be automatically reloaded.

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

class CPListItem

A selectable row in a list template.

class CPMessageListItem

A list template row that represents a conversation or contact.

