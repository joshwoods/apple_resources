

- Accelerate
-  vS1024 

Structure

# vS1024

A union containing an array or structure of eight `vUInt32` vectors or thirty-two 32-bit integers, representing a 1024-bit signed integer.

macOS 10.0+

``` source
struct vS1024
```

## Topics

### Instance Properties

var s: vS1024.__Unnamed_struct_s

var vs: vS1024.__Unnamed_struct_vs

var v: (vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32)

var s: vS1024.__Unnamed_struct_s

var vs: vS1024.__Unnamed_struct_vs

### Miscellaneous

var v: (vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32)

### Initializers

init()

init(s: vS1024.__Unnamed_struct_s)

init(v: (vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32, vUInt32))

init(vs: vS1024.__Unnamed_struct_vs)

## Relationships

### Conforms To

- Sendable

## See Also

### Data types

struct vU128

A union containing one `vUInt32` vector or four 32-bit integers, representing a 128-bit unsigned integer.

struct vS128

A union containing one `vSInt32` vector or four 32-bit integers, representing a 128-bit signed integer.

struct vU256

A union containing an array or structure of two `vUInt32` vectors or eight 32-bit integers, representing a 256-bit unsigned integer.

struct vS256

A union containing an array or structure of two `vUInt32` vectors or eight 32-bit integers, representing a 256-bit signed integer.

struct vU512

A union containing an array or structure of four `vUInt32` vectors or sixteen 32-bit integers, representing a 256-bit unsigned integer.

struct vS512

A union containing an array or structure of four `vUInt32` vectors or sixteen 32-bit integers, representing a 256-bit signed integer.

struct vU1024

A union containing an array or structure of eight `vUInt32` vectors or thirty-two 32-bit integers, representing a 1024-bit unsigned integer.

