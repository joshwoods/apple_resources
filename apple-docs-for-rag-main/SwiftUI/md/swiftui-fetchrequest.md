

- SwiftUI
-  FetchRequest 

Structure

# FetchRequest

A property wrapper type that retrieves entities from a Core Data persistent store.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @propertyWrapper @preconcurrency
struct FetchRequest where Result : NSFetchRequestResult
```

## Overview

Use a `FetchRequest` property wrapper to declare a FetchedResults property that provides a collection of Core Data managed objects to a SwiftUI view. The request infers the entity type from the `Result` placeholder type that you specify. Condition the request with an optional predicate and sort descriptors. For example, you can create a request to list all `Quake` managed objects that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data, sorted by their `time` property:

```
@FetchRequest(sortDescriptors: [SortDescriptor(\.time, order: .reverse)])
private var quakes: FetchedResults // Define Quake in your model.
```

Alternatively, when you need more flexibility, you can initialize the request with a configured NSFetchRequest instance:

```
@FetchRequest(fetchRequest: request)
private var quakes: FetchedResults
```

Always declare properties that have a fetch request wrapper as private. This lets the compiler help you avoid accidentally setting the property from the memberwise initializer of the enclosing view.

The fetch request and its results use the managed object context stored in the environment, which you can access using the managedObjectContext environment value. To support user interface activity, you typically rely on the viewContext property of a shared NSPersistentContainer instance. For example, you can set a context on your top level content view using a shared container that you define as part of your model:

```
ContentView()
    .environment(
        \.managedObjectContext,
        QuakesProvider.shared.container.viewContext)
```

When you need to dynamically change the predicate or sort descriptors, access the request’s FetchRequest.Configuration structure. To create a request that groups the fetched results according to a characteristic that they share, use SectionedFetchRequest instead.

## Topics

### Creating a fetch request

init(sortDescriptors:predicate:animation:)

Creates a fetch request based on a predicate and reference type sort parameters.

init(entity: NSEntityDescription, sortDescriptors: [NSSortDescriptor], predicate: NSPredicate?, animation: Animation?)

Creates a fetch request for a specified entity description, based on a predicate and sort parameters.

### Creating a fully configured fetch request

init(fetchRequest: NSFetchRequest&lt;Result>, animation: Animation?)

Creates a fully configured fetch request that uses the specified animation when updating results.

init(fetchRequest: NSFetchRequest&lt;Result>, transaction: Transaction)

Creates a fully configured fetch request that uses the specified transaction when updating results.

### Configuring a request dynamically

struct Configuration

The request’s configurable properties.

var projectedValue: Binding&lt;FetchRequest&lt;Result>.Configuration>

A binding to the request’s mutable configuration properties.

### Getting the fetched results

func update()

Updates the fetched results.

var wrappedValue: FetchedResults&lt;Result>

The fetched results of the fetch request.

### Default Implementations

DynamicProperty Implementations

## Relationships

### Conforms To

- Copyable
- DynamicProperty

  Conforms when `Result` conforms to `NSFetchRequestResult`.

- Sendable

## See Also

### Accessing Core Data

Loading and Displaying a Large Data Feed

Consume data in the background, and lower memory use by batching imports and preventing duplicate records.

var managedObjectContext: NSManagedObjectContext

struct FetchedResults

A collection of results retrieved from a Core Data store.

struct SectionedFetchRequest

A property wrapper type that retrieves entities, grouped into sections, from a Core Data persistent store.

struct SectionedFetchResults

A collection of results retrieved from a Core Data persistent store, grouped into sections.

