

- JavaScriptCore
-  JSObjectRef 

Type Alias

# JSObjectRef

A JavaScript object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectRef = OpaquePointer
```

## Discussion

A JSObjectRef is a JSValueRef.

## Topics

### Accessing the Global Object

func JSContextGetGlobalObject(JSContextRef!) -> JSObjectRef!

Gets the global object of a JavaScript execution context.

### Working with Objects

func JSObjectCallAsConstructor(JSContextRef!, JSObjectRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Calls an object as a constructor.

func JSObjectCallAsFunction(JSContextRef!, JSObjectRef!, JSObjectRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Calls an object as a function.

func JSObjectCopyPropertyNames(JSContextRef!, JSObjectRef!) -> JSPropertyNameArrayRef!

Gets the names of an object’s enumerable properties.

func JSObjectDeleteProperty(JSContextRef!, JSObjectRef!, JSStringRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Deletes a property from an object.

func JSObjectGetPrivate(JSObjectRef!) -> UnsafeMutableRawPointer!

Gets an object’s private data.

func JSObjectGetProperty(JSContextRef!, JSObjectRef!, JSStringRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Gets a property from an object.

func JSObjectGetPropertyAtIndex(JSContextRef!, JSObjectRef!, UInt32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Gets a property from an object by numeric index.

func JSObjectGetPrototype(JSContextRef!, JSObjectRef!) -> JSValueRef!

Gets an object’s prototype.

func JSObjectHasProperty(JSContextRef!, JSObjectRef!, JSStringRef!) -> Bool

Tests whether an object has a specified property.

func JSObjectIsConstructor(JSContextRef!, JSObjectRef!) -> Bool

Tests whether you can call an object as a constructor.

func JSObjectIsFunction(JSContextRef!, JSObjectRef!) -> Bool

Tests whether you can call an object as a function.

func JSObjectMake(JSContextRef!, JSClassRef!, UnsafeMutableRawPointer!) -> JSObjectRef!

Creates a JavaScript object.

func JSObjectMakeArray(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array object.

func JSObjectMakeConstructor(JSContextRef!, JSClassRef!, JSObjectCallAsConstructorCallback!) -> JSObjectRef!

Creates a JavaScript constructor.

func JSObjectMakeDate(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript date object as though invoking the built-in date constructor.

func JSObjectMakeError(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript error object as though invoking the built-in error constructor.

func JSObjectMakeFunction(JSContextRef!, JSStringRef!, UInt32, UnsafePointer&lt;JSStringRef?>!, JSStringRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a function with a specified script as its body.

func JSObjectMakeFunctionWithCallback(JSContextRef!, JSStringRef!, JSObjectCallAsFunctionCallback!) -> JSObjectRef!

Creates a JavaScript function with a specified callback as its implementation.

func JSObjectMakeRegExp(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript regular expression object as though invoking the built-in regular expression constructor.

func JSObjectSetPrivate(JSObjectRef!, UnsafeMutableRawPointer!) -> Bool

Sets a pointer to private data on an object.

func JSObjectSetProperty(JSContextRef!, JSObjectRef!, JSStringRef!, JSValueRef!, JSPropertyAttributes, UnsafeMutablePointer&lt;JSValueRef?>!)

Sets a property on an object.

func JSObjectSetPropertyAtIndex(JSContextRef!, JSObjectRef!, UInt32, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!)

Sets a property on an object by numeric index.

func JSObjectGetPropertyForKey(JSContextRef!, JSObjectRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Gets a property from an object using a JavaScript value as the property key.

func JSObjectSetPrototype(JSContextRef!, JSObjectRef!, JSValueRef!)

Sets an object’s prototype.

func JSObjectDeletePropertyForKey(JSContextRef!, JSObjectRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Deletes a property from an object using a JavaScript value as the property key.

func JSObjectHasPropertyForKey(JSContextRef!, JSObjectRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether an object has the specified property using a JavaScript value as the property key.

func JSObjectSetPropertyForKey(JSContextRef!, JSObjectRef!, JSValueRef!, JSValueRef!, JSPropertyAttributes, UnsafeMutablePointer&lt;JSValueRef?>!)

Sets a property on an object using a JavaScript value as the property key.

func JSObjectMakeDeferredPromise(JSContextRef!, UnsafeMutablePointer&lt;JSObjectRef?>!, UnsafeMutablePointer&lt;JSObjectRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript promise object by invoking the provided executor.

### Working with Classes

func JSClassCreate(UnsafePointer&lt;JSClassDefinition>!) -> JSClassRef!

Creates a JavaScript class.

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

func JSClassRetain(JSClassRef!) -> JSClassRef!

Retains a JavaScript class.

let kJSClassDefinitionEmpty: JSClassDefinition

A class definition structure of the current version that contains null pointers and has no attributes.

struct JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

JSClassAttribute

A JavaScript class attribute.

### Working with Properties

func JSPropertyNameAccumulatorAddName(JSPropertyNameAccumulatorRef!, JSStringRef!)

Adds a property name to a JavaScript property name accumulator.

func JSPropertyNameArrayGetCount(JSPropertyNameArrayRef!) -> Int

Gets a count of the number of items in a JavaScript property name array.

func JSPropertyNameArrayGetNameAtIndex(JSPropertyNameArrayRef!, Int) -> JSStringRef!

Gets a property name at a specified index in a JavaScript property name array.

func JSPropertyNameArrayRelease(JSPropertyNameArrayRef!)

Releases a JavaScript property name array.

func JSPropertyNameArrayRetain(JSPropertyNameArrayRef!) -> JSPropertyNameArrayRef!

Retains a JavaScript property name array.

typealias JSPropertyAttributes

A set of JavaScript property attributes.

JSPropertyAttribute

A JavaScript property attribute.

typealias JSPropertyNameArrayRef

An array of JavaScript property names.

typealias JSPropertyNameAccumulatorRef

An ordered set of the names of a JavaScript object’s properties.

### Creating a Typed Array

func JSObjectMakeTypedArray(JSContextRef!, JSTypedArrayType, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object with the specified number of elements.

func JSObjectMakeTypedArrayWithBytesNoCopy(JSContextRef!, JSTypedArrayType, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing pointer.

func JSObjectMakeTypedArrayWithArrayBuffer(JSContextRef!, JSTypedArrayType, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing JavaScript array buffer object.

func JSObjectMakeTypedArrayWithArrayBufferAndOffset(JSContextRef!, JSTypedArrayType, JSObjectRef!, Int, Int, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript typed array object from an existing JavaScript array buffer object with the specified offset and length.

struct JSTypedArrayType

The type of a JavaScript typed array object.

typealias JSTypedArrayBytesDeallocator

A function that deallocates bytes that pass to a typed array constructor.

### Accessing Typed Array Information

func JSObjectGetTypedArrayBytesPtr(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> UnsafeMutableRawPointer!

Returns a temporary pointer to the backing store of a JavaScript typed array object.

func JSObjectGetTypedArrayLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteOffset(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte offset of a JavaScript typed array object.

func JSObjectGetTypedArrayBuffer(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Returns the JavaScript array buffer object to use as the backing of a JavaScript typed array object.

### Working with Array Buffers

func JSObjectMakeArrayBufferWithBytesNoCopy(JSContextRef!, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array buffer object from an existing pointer.

func JSObjectGetArrayBufferByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the number of bytes in a JavaScript data object.

func JSObjectGetArrayBufferBytesPtr(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> UnsafeMutableRawPointer!

Returns a pointer to the data buffer that serves as the backing store for a JavaScript typed array object.

## See Also

### JavaScript Data Types

typealias JSValueRef

A JavaScript value.

