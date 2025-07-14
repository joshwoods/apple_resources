

- JavaScriptCore
-  JSObjectMake(\_:\_:\_:) 

Function

# JSObjectMake(\_:\_:\_:)

Creates a JavaScript object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectMake(
    _ ctx: JSContextRef!,
    _ jsClass: JSClassRef!,
    _ data: UnsafeMutableRawPointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`jsClass`  

The JSClassRef to assign to the object. Pass `NULL` to use the default object class.

`data`  

A pointer to set as the object’s private data. Pass `NULL` to specify no private data.

## Return Value

A JSObjectRef with the specified class and private data.

## Discussion

The default object class doesn’t allocate storage for private data, so you must provide a non-`NULL` `jsClass` to JSObjectMake(_:_:_:) if you want your object to be able to store private data.

The system sets `data` on the created object before calling the initialize methods in its class chain. This enables the initialize methods to retrieve and manipulate data through JSObjectGetPrivate(_:).

## See Also

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

func JSObjectMakeArray(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array object.

func JSObjectMakeConstructor(JSContextRef!, JSClassRef!, JSObjectCallAsConstructorCallback!) -> JSObjectRef!

Creates a JavaScript constructor.

func JSObjectMakeDate(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript date object as though invoking the built-in date constructor.

func JSObjectMakeError(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript error object as though invoking the built-in error constructor.

