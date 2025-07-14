

- CarPlay
- CPListSection
-  init(items:header:headerSubtitle:headerImage:headerButton:sectionIndexTitle:) 

Initializer

# init(items:header:headerSubtitle:headerImage:headerButton:sectionIndexTitle:)

Creates a section with list items, a header, a section index title, and section header details.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(
    items: [any CPListTemplateItem],
    header: String,
    headerSubtitle: String?,
    headerImage: UIImage?,
    headerButton: CPButton?,
    sectionIndexTitle: String?
)
```

## Parameters 

`items`  

A list of items to include in the section.

`header`  

The section header text.

`sectionIndexTitle`  

A section index title. The system displays only the first character of the title, so choose a single-character section index title.

## Return Value

A newly initialized list section.

## See Also

### Creating a Section

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

