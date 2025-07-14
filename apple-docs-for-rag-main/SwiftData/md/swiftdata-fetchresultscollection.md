

- SwiftData
-  FetchResultsCollection 

Structure

# FetchResultsCollection

A collection that efficiently provides the results of a completed fetch.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct FetchResultsCollection
```

## Topics

### Accessing a specific result

subscript(Int) -> Element

Accesses the element at the specified position.

### Accessing indices

var startIndex: Int

The position of the first element in a nonempty collection.

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

### Type Aliases

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sequence

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

func enumerate&lt;T>(FetchDescriptor&lt;T>, batchSize: Int, allowEscapingMutations: Bool, block: (T) throws -> Void) throws

Runs a closure for each model that matches the criteria of the specified fetch descriptor.

func model(for: PersistentIdentifier) -> any PersistentModel

Returns the persistent model for the specified identifier.

func registeredModel&lt;T>(for: PersistentIdentifier) -> T?

Returns the typed model for the specified identifier.

