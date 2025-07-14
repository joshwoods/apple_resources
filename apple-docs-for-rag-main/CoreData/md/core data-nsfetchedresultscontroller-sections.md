

- Core Data
- NSFetchedResultsController
-  sections 

Instance Property

# sections

The sections for the fetch results.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sections: [any NSFetchedResultsSectionInfo]? { get }
```

## Discussion

The objects in the sections array implement the NSFetchedResultsSectionInfo protocol.

You typically use the sections array when implementing `UITableViewDataSource` methods, such as numberOfSections(in:) and tableView(_:titleForHeaderInSection:).

## See Also

### Querying Section Information

func section(forSectionIndexTitle: String, at: Int) -> Int

Returns the section number for a given section title and index in the section index.

