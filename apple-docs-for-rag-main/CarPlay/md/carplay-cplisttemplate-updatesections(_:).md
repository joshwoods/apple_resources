

- CarPlay
- CPListTemplate
-  updateSections(\_:) 

Instance Method

# updateSections(\_:)

Adds, removes, reorders, or updates the list’s sections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func updateSections(_ sections: [CPListSection])
```

## Parameters 

`sections`  

An array of sections to display.

## Discussion

This method is multipurpose. Use it to add new sections to the list, to remove or reorder existing sections, and to update a section’s appearance. At runtime, use maximumSectionCount to determine the maximum number of sections the list can display. CarPlay trims the array if its size exceeds this limit.

## See Also

### Managing Sections

class var maximumSectionCount: Int

The maximum number of sections that the template can display.

var sectionCount: Int

The number of sections in the list.

var sections: [CPListSection]

The sections that the list displays.

class CPListSection

A container that groups your list items into sections.

