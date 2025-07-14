

- Accelerate
-  BNNSNDArrayFlags 

Structure

# BNNSNDArrayFlags

Options that control the behavior of an n-dimensional array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSNDArrayFlags
```

## Topics

### N-Dimensional Array Flags

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSNDArrayFlagBackpropAccumulate: BNNSNDArrayFlags

A flag that indicates backpropagation adds the value of the Jacobian to the elements of this n-dimensional array.

var BNNSNDArrayFlagBackpropSet: BNNSNDArrayFlags

A flag that indicates the elements of this n-dimensional array are overwritten by the Jacobian during backpropagation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

