

- CarPlay
- CPListTemplate
-  sectionCount 

Instance Property

# sectionCount

The number of sections in the list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var sectionCount: Int { get }
```

## Discussion

This value never exceeds maximumSectionCount. If you initialize a list, or call the updateSections(_:) method, with an array larger than `maximumSectionCount`, CarPlay trims the array to an appropriate size.

## See Also

### Managing Sections

class var maximumSectionCount: Int

The maximum number of sections that the template can display.

var sections: [CPListSection]

The sections that the list displays.

func updateSections([CPListSection])

Adds, removes, reorders, or updates the list’s sections.

class CPListSection

A container that groups your list items into sections.

