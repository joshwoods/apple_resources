

- Core Data
- NSFetchIndexDescription
-  entity 

Instance Property

# entity

The entity description for the fetch index description.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
unowned(unsafe) var entity: NSEntityDescription? { get }
```

## See Also

### Inspecting an Index Description

var elements: [NSFetchIndexElementDescription]

An array of fetch index element descriptions.

var name: String

The name of the fetch index description.

var partialIndexPredicate: NSPredicate?

A predicate that selects rows for indexing, if the index is a partial index.

