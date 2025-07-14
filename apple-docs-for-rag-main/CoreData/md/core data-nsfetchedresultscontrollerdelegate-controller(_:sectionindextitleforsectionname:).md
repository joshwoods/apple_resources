

- Core Data
- NSFetchedResultsControllerDelegate
-  controller(\_:sectionIndexTitleForSectionName:) 

Instance Method

# controller(\_:sectionIndexTitleForSectionName:)

Returns the name for a given section.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
optional func controller(
    _ controller: NSFetchedResultsController,
    sectionIndexTitleForSectionName sectionName: String
) -> String?
```

## Parameters 

`controller`  

The fetched results controller that sent the message.

`sectionName`  

The default name of the section.

## Return Value

The string to use as the name for the specified section.

## Discussion

This method does not enable change tracking. It is only needed if a section index is used.

If the delegate doesn’t implement this method, the default implementation returns the capitalized first letter of the section name (see sectionIndexTitle(forSectionName:) in `NSFetchedResultsController`).

