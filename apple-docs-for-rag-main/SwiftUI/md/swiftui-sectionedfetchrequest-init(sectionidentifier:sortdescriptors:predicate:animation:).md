

- SwiftUI
- SectionedFetchRequest
-  init(sectionIdentifier:sortDescriptors:predicate:animation:) 

Initializer

# init(sectionIdentifier:sortDescriptors:predicate:animation:)

Creates a sectioned fetch request based on a section identifier, a predicate, and reference type sort parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
init(
    sectionIdentifier: KeyPath,
    sortDescriptors: [NSSortDescriptor],
    predicate: NSPredicate? = nil,
    animation: Animation? = nil
)
```

Available when `SectionIdentifier` conforms to `Hashable` and `Result` inherits `NSManagedObject`.

Show all declarations

## Parameters 

`sectionIdentifier`  

A key path that SwiftUI applies to the `Result` type to get an object’s section identifier.

`sortDescriptors`  

An array of sort descriptors that define the sort order of the fetched results.

`predicate`  

An NSPredicate instance that defines logical conditions used to filter the fetched results.

`animation`  

The animation to use for user interface changes that result from changes to the fetched results.

## Discussion

The request gets the entity type from the `Result` instance by calling that managed object’s entity() type method. If you need to specify the entity type explicitly, use the init(entity:sectionIdentifier:sortDescriptors:predicate:animation:) initializer instead. If you need more control over the fetch request configuration, use init(fetchRequest:sectionIdentifier:animation:). For value type sort descriptors, use init(sectionIdentifier:sortDescriptors:predicate:animation:).

## See Also

### Creating a fetch request

init(entity: NSEntityDescription, sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>, sortDescriptors: [NSSortDescriptor], predicate: NSPredicate?, animation: Animation?)

Creates a sectioned fetch request for a specified entity description, based on a section identifier, a predicate, and sort parameters.

