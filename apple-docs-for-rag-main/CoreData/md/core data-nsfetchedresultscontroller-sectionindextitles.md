

- Core Data
- NSFetchedResultsController
-  sectionIndexTitles 

Instance Property

# sectionIndexTitles

The array of section index titles.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sectionIndexTitles: [String] { get }
```

## Discussion

The default implementation returns the array created by calling sectionIndexTitle(forSectionName:) on all the known sections. You should override this method if you want to return a different array for the section index.

### Special Considerations

You only need this method if you use a section index.

## See Also

### Configuring Section Information

func sectionIndexTitle(forSectionName: String) -> String?

Returns the corresponding section index entry for a given section name.

