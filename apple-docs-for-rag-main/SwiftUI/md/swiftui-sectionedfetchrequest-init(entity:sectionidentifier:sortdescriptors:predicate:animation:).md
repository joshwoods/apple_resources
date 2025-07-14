

- SwiftUI
- SectionedFetchRequest
-  init(entity:sectionIdentifier:sortDescriptors:predicate:animation:) 

Initializer

# init(entity:sectionIdentifier:sortDescriptors:predicate:animation:)

Creates a sectioned fetch request for a specified entity description, based on a section identifier, a predicate, and sort parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
init(
    entity: NSEntityDescription,
    sectionIdentifier: KeyPath,
    sortDescriptors: [NSSortDescriptor],
    predicate: NSPredicate? = nil,
    animation: Animation? = nil
)
```

Available when `SectionIdentifier` conforms to `Hashable` and `Result` conforms to `NSFetchRequestResult`.

## Parameters 

`entity`  

The description of the Core Data entity to fetch.

`sectionIdentifier`  

A key path that SwiftUI applies to the `Result` type to get an object’s section identifier.

`sortDescriptors`  

An array of sort descriptors that define the sort order of the fetched results.

`predicate`  

An NSPredicate instance that defines logical conditions used to filter the fetched results.

`animation`  

The animation to use for user interface changes that result from changes to the fetched results.

## Discussion

Use this initializer if you need to explicitly specify the entity type for the request. If you specify a placeholder `Result` type in the request declaration, use the init(sectionIdentifier:sortDescriptors:predicate:animation:) initializer to let the request infer the entity type. If you need more control over the fetch request configuration, use init(fetchRequest:sectionIdentifier:animation:).

## See Also

### Creating a fetch request

init(sectionIdentifier:sortDescriptors:predicate:animation:)

Creates a sectioned fetch request based on a section identifier, a predicate, and reference type sort parameters.

