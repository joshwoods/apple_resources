

- CarPlay
- CPListTemplate
-  maximumSectionCount 

Type Property

# maximumSectionCount

The maximum number of sections that the template can display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class var maximumSectionCount: Int { get }
```

## Discussion

This property’s value is dependent on any user interface limits that the vehicle imposes. See CPSessionConfiguration for more information. At runtime, use this value to determine the maximum number of sections that your list can display.

## See Also

### Managing Sections

var sectionCount: Int

The number of sections in the list.

var sections: [CPListSection]

The sections that the list displays.

func updateSections([CPListSection])

Adds, removes, reorders, or updates the list’s sections.

class CPListSection

A container that groups your list items into sections.

