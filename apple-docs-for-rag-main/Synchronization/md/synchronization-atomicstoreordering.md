

- Synchronization
-  AtomicStoreOrdering 

Structure

# AtomicStoreOrdering

Specifies the memory ordering semantics of an atomic store operation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct AtomicStoreOrdering
```

## Topics

### Type Properties

static var relaxed: AtomicStoreOrdering

Guarantees the atomicity of the specific operation on which it is applied, but imposes no ordering constraints on any other variable accesses.

static var releasing: AtomicStoreOrdering

A releasing store synchronizes with acquiring operations that read the value it stores. It ensures that the releasing and acquiring threads agree that all preceding variable accesses on the releasing thread happen before the atomic operation itself.

static var sequentiallyConsistent: AtomicStoreOrdering

A sequentially consistent store performs a releasing store and also guarantees that it and all other sequentially consistent atomic operations (loads, stores, updates) appear to be executed in a single, total sequential ordering.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Memory Ordering Semantics

struct AtomicLoadOrdering

Specifies the memory ordering semantics of an atomic load operation.

struct AtomicUpdateOrdering

Specifies the memory ordering semantics of an atomic read-modify-write operation.

func atomicMemoryFence(ordering: AtomicUpdateOrdering)

Establishes a memory ordering without associating it with a particular atomic operation.

