

- Accelerate
-  BNNSFilterDestroy(\_:) Deprecated

Function

# BNNSFilterDestroy(\_:)

Destroys the specified filter, releasing all resources allocated for it.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.12–15.0DeprecatedtvOS 10.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
func BNNSFilterDestroy(_ filter: BNNSFilter?)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

A BNNSFilter object.

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

typealias BNNSAlloc

A type-alias for a user-provided memory allocation function.

typealias BNNSFree

A type-alias for a user-provided memory deallocation function.

