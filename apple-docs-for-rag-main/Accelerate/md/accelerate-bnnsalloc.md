

- Accelerate
-  BNNSAlloc 

Type Alias

# BNNSAlloc

A type-alias for a user-provided memory allocation function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias BNNSAlloc = (UnsafeMutablePointer?, Int, Int) -> Int32
```

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

struct BNNSFilterParameters

A structure that contains common filter parameters.

func BNNSFilterDestroy(BNNSFilter?)

Destroys the specified filter, releasing all resources allocated for it.

Deprecated

typealias BNNSFree

A type-alias for a user-provided memory deallocation function.

