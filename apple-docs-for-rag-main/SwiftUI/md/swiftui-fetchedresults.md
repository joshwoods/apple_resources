

- SwiftUI
-  FetchedResults 

Structure

# FetchedResults

A collection of results retrieved from a Core Data store.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
struct FetchedResults where Result : NSFetchRequestResult
```

## Overview

Use a `FetchedResults` instance to show or edit Core Data managed objects in your app’s user interface. You request a particular set of results by specifying a `Result` type as the entity type, and annotating the fetched results property declaration with a FetchRequest property wrapper. For example, you can create a request to list all `Quake` managed objects that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data, sorted by their `time` property:

```
@FetchRequest(sortDescriptors: [SortDescriptor(\.time, order: .reverse)])
private var quakes: FetchedResults
```

The results instance conforms to RandomAccessCollection, so you access it like any other collection. For example, you can create a List that iterates over all the results:

```
List(quakes) { quake in
    NavigationLink(destination: QuakeDetail(quake: quake)) {
        QuakeRow(quake: quake)
    }
}
```

When you need to dynamically change the request’s predicate or sort descriptors, set the result instance’s nsPredicate and sortDescriptors or nsSortDescriptors properties, respectively.

The fetch request and its results use the managed object context stored in the environment, which you can access using the managedObjectContext environment value. To support user interface activity, you typically rely on the viewContext property of a shared NSPersistentContainer instance. For example, you can set a context on your top level content view using a container that you define as part of your model:

```
ContentView()
    .environment(
        \.managedObjectContext,
        QuakesProvider.shared.container.viewContext)
```

## Topics

### Configuring the associated fetch request

var nsPredicate: NSPredicate?

The request’s predicate.

var sortDescriptors: [SortDescriptor&lt;Result>]

The request’s sort descriptors, accessed as value types.

var nsSortDescriptors: [NSSortDescriptor]

The request’s sort descriptors, accessed as reference types.

### Getting indices

var startIndex: Int

The index of the first entity in the results collection.

var endIndex: Int

The index that’s one greater than the last valid subscript argument.

### Getting results

subscript(Int) -> Result

Gets the entity at the specified index.

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

struct SectionedFetchRequest

A property wrapper type that retrieves entities, grouped into sections, from a Core Data persistent store.

struct SectionedFetchResults

A collection of results retrieved from a Core Data persistent store, grouped into sections.

