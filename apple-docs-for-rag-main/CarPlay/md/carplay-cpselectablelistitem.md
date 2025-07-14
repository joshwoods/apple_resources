

- CarPlay
-  CPSelectableListItem 

Protocol

# CPSelectableListItem

A description of a selectable list item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol CPSelectableListItem : CPListTemplateItem
```

## Overview

Important

You don’t create custom classes that conform to `CPSelectableListItem`. Instead, you use one of the prebuilt list item types that adopt this protocol, such as CPListItem or CPListImageRowItem.

## Topics

### Managing Selection

var handler: ((any CPSelectableListItem, () -> Void) -> Void)?

An optional closure that CarPlay invokes when the user selects the list item.

**Required**

## Relationships

### Inherits From

- CPListTemplateItem
- NSObjectProtocol

### Conforming Types

- CPListImageRowItem
- CPListItem

## See Also

### Creating a Section

init(items: [any CPListTemplateItem], header: String, headerSubtitle: String?, headerImage: UIImage?, headerButton: CPButton?, sectionIndexTitle: String?)

Creates a section with list items, a header, a section index title, and section header details.

protocol CPListTemplateItem

A description of the common properties of all list item types.

class CPListItem

A selectable row in a list template.

class CPListImageRowItem

A list template row that displays a series of images.

class CPMessageListItem

A list template row that represents a conversation or contact.

