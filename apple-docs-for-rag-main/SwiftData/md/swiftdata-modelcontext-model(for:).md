

- SwiftData
- ModelContext
-  model(for:) 

Instance Method

# model(for:)

Returns the persistent model for the specified identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func model(for persistentModelID: PersistentIdentifier) -> any PersistentModel
```

## Parameters 

`persistentModelID`  

The identifier of the model to fetch. For more information, see PersistentIdentifier.

## Return Value

The identified persistent model, if known to the context; otherwise, an unsaved model with its persistentModelID property set to `persistentModelID`.

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

func enumerate&lt;T>(FetchDescriptor&lt;T>, batchSize: Int, allowEscapingMutations: Bool, block: (T) throws -> Void) throws

Runs a closure for each model that matches the criteria of the specified fetch descriptor.

func registeredModel&lt;T>(for: PersistentIdentifier) -> T?

Returns the typed model for the specified identifier.

