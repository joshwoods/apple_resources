

- JavaScriptCore
-  JSTypedArrayType 

Structure

# JSTypedArrayType

The type of a JavaScript typed array object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
struct JSTypedArrayType
```

## Topics

### Constants

var kJSTypedArrayTypeNone: JSTypedArrayType

Not a typed array.

var kJSTypedArrayTypeArrayBuffer: JSTypedArrayType

An array buffer type.

var kJSTypedArrayTypeInt8Array: JSTypedArrayType

An 8-bit integer array type.

var kJSTypedArrayTypeInt16Array: JSTypedArrayType

A 16-bit integer array type.

var kJSTypedArrayTypeInt32Array: JSTypedArrayType

A 32-bit integer array type.

var kJSTypedArrayTypeBigInt64Array: JSTypedArrayType

var kJSTypedArrayTypeUint8Array: JSTypedArrayType

An 8-bit unsigned integer array type.

var kJSTypedArrayTypeUint8ClampedArray: JSTypedArrayType

An 8-bit unsigned integer clamped array type.

var kJSTypedArrayTypeUint16Array: JSTypedArrayType

A 16-bit unsigned integer array type.

var kJSTypedArrayTypeUint32Array: JSTypedArrayType

A 32-bit unsigned integer array type.

var kJSTypedArrayTypeBigUint64Array: JSTypedArrayType

var kJSTypedArrayTypeFloat32Array: JSTypedArrayType

A 32-bit floating point array type.

var kJSTypedArrayTypeFloat64Array: JSTypedArrayType

A 64-bit floating point array type.

### Initializers

init(UInt32)

Creates a typed array.

init(rawValue: UInt32)

Creates a typed array with the specified raw value.

var rawValue: UInt32

The raw value that represents the typed array’s type.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Typed Array

func JSObjectMakeTypedArray(JSContextRef!, JSTypedArrayType, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object with the specified number of elements.

func JSObjectMakeTypedArrayWithBytesNoCopy(JSContextRef!, JSTypedArrayType, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing pointer.

func JSObjectMakeTypedArrayWithArrayBuffer(JSContextRef!, JSTypedArrayType, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing JavaScript array buffer object.

func JSObjectMakeTypedArrayWithArrayBufferAndOffset(JSContextRef!, JSTypedArrayType, JSObjectRef!, Int, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing JavaScript array buffer object with the specified offset and length.

typealias JSTypedArrayBytesDeallocator

A function that deallocates bytes that pass to a typed array constructor.

