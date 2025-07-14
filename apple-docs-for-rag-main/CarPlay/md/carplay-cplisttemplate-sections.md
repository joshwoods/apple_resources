

- CarPlay
- CPListTemplate
-  sections 

Instance Property

# sections

The sections that the list displays.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var sections: [CPListSection] { get }
```

## Discussion

To add new sections to the list, to remove or reorder existing sections, or to update a section’s appearance, use the updateSections(_:) method.

## See Also

### Managing Sections

class var maximumSectionCount: Int

The maximum number of sections that the template can display.

var sectionCount: Int

The number of sections in the list.

func updateSections([CPListSection])

Adds, removes, reorders, or updates the list’s sections.

class CPListSection

A container that groups your list items into sections.

