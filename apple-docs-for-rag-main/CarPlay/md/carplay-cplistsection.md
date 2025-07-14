

- CarPlay
-  CPListSection 

Class

# CPListSection

A container that groups your list items into sections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPListSection
```

## Overview

A section contains zero or more list items. You can configure a section to display a header and a section index title, which CarPlay displays on the trailing edge of the screen. The section header and the section index title are optional.

To create a section, call the initWithItems: method and provide an array of list items. Alternatively, use initWithItems:header:sectionIndexTitle: if you want to display a header and a section index title. CarPlay doesn’t support custom list items, so you must use one of the types that the framework provides, such as CPListItem or CPListImageRowItem.

At runtime, use maximumSectionCount to determine the maximum number of sections that your list can display. When creating items for your sections, use maximumItemCount to establish the maximum number of items across all sections that can appear in your list.

## Topics

### Creating a Section

init(items: [any CPListTemplateItem], header: String, headerSubtitle: String?, headerImage: UIImage?, headerButton: CPButton?, sectionIndexTitle: String?)

Creates a section with list items, a header, a section index title, and section header details.

protocol CPListTemplateItem

A description of the common properties of all list item types.

protocol CPSelectableListItem

A description of a selectable list item.

class CPListItem

A selectable row in a list template.

class CPListImageRowItem

A list template row that displays a series of images.

class CPMessageListItem

A list template row that represents a conversation or contact.

### Getting Supplementary Information

var header: String?

The section’s header text.

var sectionIndexTitle: String?

The section’s index title.

### Getting Items

var items: [any CPListTemplateItem]

The list of items for the section.

func index(of: any CPListTemplateItem) -> Int

Returns the index of the specified item.

func item(at: Int) -> any CPListTemplateItem

Returns the item at the specified index.

### Configuring Section Headers

var headerButton: CPButton?

A button that the section header displays.

var headerImage: UIImage?

An image that the section header displays.

var headerSubtitle: String?

A string that the header displays as a subtitle.

### Initializers

convenience init(items: [CPListItem])

convenience init(items: [CPListItem], header: String?, sectionIndexTitle: String?)

convenience init(items: [any CPListTemplateItem])

convenience init(items: [any CPListTemplateItem], header: String?, sectionIndexTitle: String?)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing Sections

class var maximumSectionCount: Int

The maximum number of sections that the template can display.

var sectionCount: Int

The number of sections in the list.

var sections: [CPListSection]

The sections that the list displays.

func updateSections([CPListSection])

Adds, removes, reorders, or updates the list’s sections.

