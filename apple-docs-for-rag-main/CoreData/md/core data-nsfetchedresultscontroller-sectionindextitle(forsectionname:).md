

- Core Data
- NSFetchedResultsController
-  sectionIndexTitle(forSectionName:) 

Instance Method

# sectionIndexTitle(forSectionName:)

Returns the corresponding section index entry for a given section name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func sectionIndexTitle(forSectionName sectionName: String) -> String?
```

## Parameters 

`sectionName`  

The name of a section.

## Return Value

The section index entry corresponding to the section with name `sectionName`.

## Discussion

The default implementation returns the capitalized first letter of the section name.

You should override this method if you need a different way to convert from a section name to its name in the section index.

### Special Considerations

You only need this method if you use a section index.

## See Also

### Configuring Section Information

var sectionIndexTitles: [String]

The array of section index titles.

