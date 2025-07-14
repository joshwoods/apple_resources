

- Accelerate
-  bnns_graph_argument_t 

Structure

# bnns_graph_argument_t

Describes data associated with an input or output argument

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct bnns_graph_argument_t
```

## Overview

Exactly one of descriptor or data_ptr should be set based on the configuration specified with `BNNSGraphContextSetArgumentType()`

## Topics

### Initializers

init()

### Instance Properties

var data_ptr: UnsafeMutableRawPointer?

var data_ptr_size: Int

size in bytes of `data_ptr`, if set

var descriptor: UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?

var tensor: UnsafeMutablePointer&lt;BNNSTensor>?

## Relationships

### Conforms To

- Sendable

## See Also

### Structures

struct BNNSDataType

BNNS Data Types.

struct BNNSSparsityParameters

struct BNNSSparsityType

struct BNNSTargetSystem

struct BNNSImageStackDescriptorDeprecated

struct BNNSVectorDescriptorDeprecated

