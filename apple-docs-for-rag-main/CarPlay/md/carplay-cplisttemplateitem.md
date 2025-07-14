

- CarPlay
-  CPListTemplateItem 

Protocol

# CPListTemplateItem

A description of the common properties of all list item types.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol CPListTemplateItem : NSObjectProtocol
```

## Overview

Important

You don’t create custom classes that conform to `CPListItemTemplate`. Instead, you use one of the prebuilt list item types that adopt this protocol, such as CPMessageListItem.

## Topics

### Managing Content

var text: String?

The item’s primary text.

**Required**

var userInfo: Any?

An opaque value for the list item.

**Required**

### Enabling Items

var isEnabled: Bool

A Boolean value that indicates if the item is enabled.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- CPSelectableListItem

### Conforming Types

- CPListImageRowItem
- CPListItem
- CPMessageListItem

## See Also

### Creating a Section

init(items: [any CPListTemplateItem], header: String, headerSubtitle: String?, headerImage: UIImage?, headerButton: CPButton?, sectionIndexTitle: String?)

Creates a section with list items, a header, a section index title, and section header details.

protocol CPSelectableListItem

A description of a selectable list item.

class CPListItem

A selectable row in a list template.

class CPListImageRowItem

A list template row that displays a series of images.

class CPMessageListItem

A list template row that represents a conversation or contact.

