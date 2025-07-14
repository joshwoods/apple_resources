

- SwiftData
- ModelContext
-  enumerate(\_:batchSize:allowEscapingMutations:block:) 

Instance Method

# enumerate(\_:batchSize:allowEscapingMutations:block:)

Runs a closure for each model that matches the criteria of the specified fetch descriptor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func enumerate(
    _ fetch: FetchDescriptor,
    batchSize: Int = 5000,
    allowEscapingMutations: Bool = false,
    block: (T) throws -> Void
) throws where T : PersistentModel
```

## Parameters 

`fetch`  

A fetch descriptor that provides the configuration for the fetch.

`batchSize`  

The maximum number of models to include in each batch. The default value is 5000.

`allowEscapingMutations`  

A Boolean value that determines whether the closure can leave the context in a modified state after it completes. The default value is `false`.

`block`  

The closure to run for each fetched model.

## See Also

### Fetching models

func fetch&lt;T>(FetchDescriptor&lt;T>) throws -> [T]

Returns an array of typed models that match the criteria of the specified fetch descriptor.

func fetch&lt;T>(FetchDescriptor&lt;T>, batchSize: Int) throws -> FetchResultsCollection&lt;T>

Returns a collection of typed models, in batches, which match the criteria of the specified fetch descriptor.

func fetchCount&lt;T>(FetchDescriptor&lt;T>) throws -> Int

Returns the number of models that match the criteria of the specified fetch descriptor.

struct FetchDescriptor

A type that describes the criteria, sort order, and any additional configuration to use when performing a fetch.

struct FetchResultsCollection

A collection that efficiently provides the results of a completed fetch.

func model(for: PersistentIdentifier) -> any PersistentModel

Returns the persistent model for the specified identifier.

func registeredModel&lt;T>(for: PersistentIdentifier) -> T?

Returns the typed model for the specified identifier.

