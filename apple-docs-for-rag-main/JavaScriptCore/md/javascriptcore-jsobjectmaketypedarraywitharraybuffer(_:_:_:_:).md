

- JavaScriptCore
-  JSObjectMakeTypedArrayWithArrayBuffer(\_:\_:\_:\_:) 

Function

# JSObjectMakeTypedArrayWithArrayBuffer(\_:\_:\_:\_:)

Creates a JavaScript typed array object from an existing JavaScript array buffer object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectMakeTypedArrayWithArrayBuffer(
    _ ctx: JSContextRef!,
    _ arrayType: JSTypedArrayType,
    _ buffer: JSObjectRef!,
    _ exception: UnsafeMutablePointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`arrayType`  

A value that identifies the type of array to create. If `arrayType` is kJSTypedArrayTypeNone or kJSTypedArrayTypeArrayBuffer, this function returns `NULL`.

`buffer`  

An array buffer object to use as the backing store for the created JavaScript typed array object.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` if you don’t want to store an exception.

## Return Value

A JSObjectRef that is a typed array, or `NULL` if there is an error. The backing store of the typed array is `buffer`.

## See Also

### Creating a Typed Array

func JSObjectMakeTypedArray(JSContextRef!, JSTypedArrayType, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object with the specified number of elements.

func JSObjectMakeTypedArrayWithBytesNoCopy(JSContextRef!, JSTypedArrayType, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing pointer.

func JSObjectMakeTypedArrayWithArrayBufferAndOffset(JSContextRef!, JSTypedArrayType, JSObjectRef!, Int, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing JavaScript array buffer object with the specified offset and length.

struct JSTypedArrayType

The type of a JavaScript typed array object.

typealias JSTypedArrayBytesDeallocator

A function that deallocates bytes that pass to a typed array constructor.

