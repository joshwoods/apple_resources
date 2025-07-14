

- Accelerate
-  vR1024Rotate(\_:\_:\_:) 

Function

# vR1024Rotate(\_:\_:\_:)

1024-bit right rotate.

macOS 10.0+

``` source
func vR1024Rotate(
    _ a: UnsafePointer,
    _ rotateAmount: UInt32,
    _ result: UnsafeMutablePointer
)
```

## See Also

### Shifting and rotating large integers

func vLL256Shift(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit logical left shift.

func vLR256Shift(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit logical right shift.

func vA256Shift(UnsafePointer&lt;vS256>, UInt32, UnsafeMutablePointer&lt;vS256>)

256-bit arithmetic shift.

func vLL512Shift(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit logical left shift.

func vLR512Shift(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit logical right shift .

func vA512Shift(UnsafePointer&lt;vS512>, UInt32, UnsafeMutablePointer&lt;vS512>)

512-bit arithmetic shift.

func vLL1024Shift(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit logical left shift.

func vLR1024Shift(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit logical right shift .

func vA1024Shift(UnsafePointer&lt;vS1024>, UInt32, UnsafeMutablePointer&lt;vS1024>)

1024-bit arithmetic shift.

func vL256Rotate(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit left rotate.

func vR256Rotate(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit right rotate.

func vL512Rotate(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit left rotate.

func vR512Rotate(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit right rotate.

func vL1024Rotate(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit left rotate.

