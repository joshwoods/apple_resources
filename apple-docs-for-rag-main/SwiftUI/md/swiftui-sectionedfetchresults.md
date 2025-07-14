

- SwiftUI
-  SectionedFetchResults 

Structure

# SectionedFetchResults

A collection of results retrieved from a Core Data persistent store, grouped into sections.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
struct SectionedFetchResults where SectionIdentifier : Hashable, Result : NSFetchRequestResult
```

## Overview

Use a `SectionedFetchResults` instance to show or edit Core Data managed objects, grouped into sections, in your app’s user interface. If you don’t need sectioning, use FetchedResults instead.

You request a particular set of results by annotating the fetched results property declaration with a SectionedFetchRequest property wrapper. Indicate the type of the fetched entities with a `Results` type, and the type of the identifier that distinguishes the sections with a `SectionIdentifier` type. For example, you can create a request to list all `Quake` managed objects that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data, sorted by their `time` property and grouped by a string that represents the days when earthquakes occurred:

```
```

The `quakes` property acts as a collection of SectionedFetchResults.Section instances, each containing a collection of `Quake` instances. The example above depends on the `Quake` model object declaring both `time` and `day` properties, either stored or computed. For best performance with large data sets, use stored properties.

The collection of sections, as well as the collection of managed objects in each section, conforms to the RandomAccessCollection protocol, so you can access them as you would any other collection. For example, you can create nested ForEach loops inside a List to iterate over the results:

```
```

Don’t confuse the Section view that you use to create a hierarchical display with the SectionedFetchResults.Section instances that hold the fetched results.

When you need to dynamically change the request’s section identifier, predicate, or sort descriptors, set the result instance’s sectionIdentifier, nsPredicate, and sortDescriptors or nsSortDescriptors properties, respectively. Be sure that the sorting and sectioning work together to avoid discontinguous sections.

The fetch request and its results use the managed object context stored in the environment, which you can access using the managedObjectContext environment value. To support user interface activity, you typically rely on the viewContext property of a shared NSPersistentContainer instance. For example, you can set a context on your top-level content view using a container that you define as part of your model:

```
```

## Topics

### Configuring the associated sectioned fetch request

var nsPredicate: NSPredicate?

The request’s predicate.

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

var sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>

The key path that the system uses to group fetched results into sections.

struct Section

A collection of fetched results that share a specified identifier.

### Getting indices

var startIndex: Int

The index of the first section in the results collection.

var endIndex: Int

The index that’s one greater than that of the last section.

### Getting results

subscript(Int) -> SectionedFetchResults&lt;SectionIdentifier, Result>.Section

Gets the section at the specified index.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Accessing Core Data

Loading and Displaying a Large Data Feed

Consume data in the background, and lower memory use by batching imports and preventing duplicate records.

var managedObjectContext: NSManagedObjectContext

struct FetchRequest

A property wrapper type that retrieves entities from a Core Data persistent store.

struct FetchedResults

A collection of results retrieved from a Core Data store.

struct SectionedFetchRequest

A property wrapper type that retrieves entities, grouped into sections, from a Core Data persistent store.

