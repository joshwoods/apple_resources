

- SwiftUI
-  SectionedFetchRequest 

Structure

# SectionedFetchRequest

A property wrapper type that retrieves entities, grouped into sections, from a Core Data persistent store.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @propertyWrapper @preconcurrency
struct SectionedFetchRequest where SectionIdentifier : Hashable, Result : NSFetchRequestResult
```

## Overview

Use a `SectionedFetchRequest` property wrapper to declare a SectionedFetchResults property that provides a grouped collection of Core Data managed objects to a SwiftUI view. If you don’t need sectioning, use FetchRequest instead.

Configure a sectioned fetch request with an optional predicate and sort descriptors, and include a `sectionIdentifier` parameter to indicate how to group the fetched results. Be sure that you choose sorting and sectioning that work together to avoid discontiguous sections. For example, you can request a list of earthquakes, composed of `Quake` managed objects that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data, sorted by time and grouped by date:

```
@SectionedFetchRequest(
    sectionIdentifier: \.day,
    sortDescriptors: [SortDescriptor(\.time, order: .reverse)]
)
private var quakes: SectionedFetchResults
```

Always declare properties that have a sectioned fetch request wrapper as private. This lets the compiler help you avoid accidentally setting the property from the memberwise initializer of the enclosing view.

The request infers the entity type from the `Result` type that you specify, which is `Quake` in the example above. Indicate a `SectionIdentifier` type to declare the type found at the fetched object’s `sectionIdentifier` key path. The section identifier type must conform to the Hashable protocol.

The example above depends on the `Quake` type having a `day` property that’s either a stored or computed string. Be sure to mark any computed property with the `@objc` attribute for it to function as a section identifier. For best performance with large data sets, use stored properties.

The sectioned fetch request and its results use the managed object context stored in the environment, which you can access using the managedObjectContext environment value. To support user interface activity, you typically rely on the viewContext property of a shared NSPersistentContainer instance. For example, you can set a context on your top-level content view using a shared container that you define as part of your model:

```
ContentView()
    .environment(
        \.managedObjectContext,
        QuakesProvider.shared.container.viewContext)
```

When you need to dynamically change the section identifier, predicate, or sort descriptors, access the request’s SectionedFetchRequest.Configuration structure, either directly or with a binding.

## Topics

### Creating a fetch request

init(sectionIdentifier:sortDescriptors:predicate:animation:)

Creates a sectioned fetch request based on a section identifier, a predicate, and reference type sort parameters.

init(entity: NSEntityDescription, sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>, sortDescriptors: [NSSortDescriptor], predicate: NSPredicate?, animation: Animation?)

Creates a sectioned fetch request for a specified entity description, based on a section identifier, a predicate, and sort parameters.

### Creating a fully configured fetch request

init(fetchRequest: NSFetchRequest&lt;Result>, sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>, animation: Animation?)

Creates a fully configured sectioned fetch request that uses the specified animation when updating results.

init(fetchRequest: NSFetchRequest&lt;Result>, sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>, transaction: Transaction)

Creates a fully configured sectioned fetch request that uses the specified transaction when updating results.

### Configuring a request dynamically

struct Configuration

The request’s configurable properties.

var projectedValue: Binding&lt;SectionedFetchRequest&lt;SectionIdentifier, Result>.Configuration>

A binding to the request’s mutable configuration properties.

### Getting the fetched results

func update()

Updates the fetched results.

var wrappedValue: SectionedFetchResults&lt;SectionIdentifier, Result>

The fetched results of the fetch request.

### Default Implementations

DynamicProperty Implementations

## Relationships

### Conforms To

- Copyable
- DynamicProperty

  Conforms when `SectionIdentifier` conforms to `Hashable` and `Result` conforms to `NSFetchRequestResult`.

## See Also

### Accessing Core Data

Loading and Displaying a Large Data Feed

Consume data in the background, and lower memory use by batching imports and preventing duplicate records.

var managedObjectContext: NSManagedObjectContext

struct FetchRequest

A property wrapper type that retrieves entities from a Core Data persistent store.

struct FetchedResults

A collection of results retrieved from a Core Data store.

struct SectionedFetchResults

A collection of results retrieved from a Core Data persistent store, grouped into sections.

