

- Accelerate
-  BNNSFilterParameters 

Structure

# BNNSFilterParameters

A structure that contains common filter parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSFilterParameters
```

## Topics

### Initializers

init(options: BNNSFlags, threadCount: Int, allocator: BNNSAlloc?, deallocator: BNNSFree?)

Returns a new common filter parameters structure using the specified options.

init(flags: UInt32, n_threads: Int, alloc_memory: BNNSAlloc?, free_memory: BNNSFree?)

Returns a new common filter parameters structure.

init()

### Instance Properties

var flags: UInt32

A logical OR of zero or more values from BNNS flags.

var n_threads: Int

The number of worker threads to execute.

var alloc_memory: BNNSAlloc?

The function called to allocate memory.

var free_memory: BNNSFree?

The function called to deallocate memory.

var allocator: BNNSAlloc?

var deallocator: BNNSFree?

var options: BNNSFlags

var threadCount: Int

### Filter Flags

struct BNNSFlags

Options that control the behavior of a filter parameter.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### General filters

typealias BNNSFilter

An opaque type that represents a filter.

Deprecated

Applying Filters

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class UnaryLayer

The base class for layers that accept a single input.

Deprecated

class BinaryLayer

The base class for layers that accept two inputs.

Deprecated

func BNNSFilterDestroy(BNNSFilter?)

Destroys the specified filter, releasing all resources allocated for it.

Deprecated

typealias BNNSAlloc

A type-alias for a user-provided memory allocation function.

typealias BNNSFree

A type-alias for a user-provided memory deallocation function.

