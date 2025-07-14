

- Kernel
- Hardware Families
- Audio
-  IOAF_NativeInt16ToFloat32 

Function

# IOAF_NativeInt16ToFloat32

Converts native 16-bit integer float to 32-bit float

macOS 10.7+

``` source
void IOAF_NativeInt16ToFloat32(const SInt16 *src, Float32 *dest, unsigned int count);
```

## Parameters 

`src`  

Pointer to the data to convert

`dest`  

Pointer to the converted data

`count`  

The number of items to convert

## See Also

### Conversions

IOAF_Float32ToInt8

IOAF_Float32ToNativeInt16

Converts 32-bit floating point to native 16-bit integer

IOAF_Float32ToNativeInt24

Converts 32-bit floating point to native 24-bit integer

IOAF_Float32ToNativeInt32

Converts 32-bit floating point to native 32-bit integer

IOAF_Float32ToSwapInt16

Converts 32-bit floating point to non-native 16-bit integer

IOAF_Float32ToSwapInt24

Converts 32-bit floating point to non-native 24-bit integer

IOAF_Float32ToSwapInt32

Converts 32-bit floating point to non-native 32-bit integer

IOAF_Int8ToFloat32

IOAF_NativeInt24ToFloat32

Converts native 24-bit integer float to 32-bit float

IOAF_NativeInt32ToFloat32

Converts native 32-bit integer float to 32-bit float

IOAF_SwapInt16ToFloat32

Converts non-native 16-bit integer float to 32-bit float

IOAF_SwapInt24ToFloat32

Converts non-native 24-bit integer float to 32-bit float

IOAF_SwapInt32ToFloat32

Converts non-native 32-bit integer float to 32-bit float

