

- Core Data
- NSFetchedResultsController
-  section(forSectionIndexTitle:at:) 

Instance Method

# section(forSectionIndexTitle:at:)

Returns the section number for a given section title and index in the section index.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func section(
    forSectionIndexTitle title: String,
    at sectionIndex: Int
) -> Int
```

## Parameters 

`title`  

The title of a section

`sectionIndex`  

The index of a section.

## Return Value

The section number for the given section title and index in the section index

## Discussion

You would typically call this method when executing `UITableViewDataSource`’s tableView(_:sectionForSectionIndexTitle:at:) method.

## See Also

### Querying Section Information

var sections: [any NSFetchedResultsSectionInfo]?

The sections for the fetch results.

