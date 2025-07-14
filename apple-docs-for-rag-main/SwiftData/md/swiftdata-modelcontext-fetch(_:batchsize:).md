

- SwiftData
- ModelContext
-  fetch(\_:batchSize:) 

Instance Method

# fetch(\_:batchSize:)

Returns a collection of typed models, in batches, which match the criteria of the specified fetch descriptor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func fetch(
    _ descriptor: FetchDescriptor,
    batchSize: Int
) throws -> FetchResultsCollection where T : PersistentModel
```

## Parameters 

`descriptor`  

A fetch descriptor that provides the configuration for the fetch.

`batchSize`  

The maximum number of models to include in each batch.

## Return Value

The collection of typed models that satisfy the criteria of the fetch descriptor. If no models match the criteria, the collection is empty.

## Discussion

As you access the models in the returned collection (either sequentially, or directly using subscripting), the context automatically fetches the necessary batches.

## See Also

### Fetching models

func fetch&lt;T>(FetchDescriptor&lt;T>) throws -> [T]

Returns an array of typed models that match the criteria of the specified fetch descriptor.

func fetchCount&lt;T>(FetchDescriptor&lt;T>) throws -> Int

Returns the number of models that match the criteria of the specified fetch descriptor.

struct FetchDescriptor

A type that describes the criteria, sort order, and any additional configuration to use when performing a fetch.

struct FetchResultsCollection

A collection that efficiently provides the results of a completed fetch.

func enumerate&lt;T>(FetchDescriptor&lt;T>, batchSize: Int, allowEscapingMutations: Bool, block: (T) throws -> Void) throws

Runs a closure for each model that matches the criteria of the specified fetch descriptor.

func model(for: PersistentIdentifier) -> any PersistentModel

Returns the persistent model for the specified identifier.

func registeredModel&lt;T>(for: PersistentIdentifier) -> T?

Returns the typed model for the specified identifier.

