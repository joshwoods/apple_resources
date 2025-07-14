

- JavaScriptCore
-  JSObjectCallAsFunction(\_:\_:\_:\_:\_:\_:) 

Function

# JSObjectCallAsFunction(\_:\_:\_:\_:\_:\_:)

Calls an object as a function.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectCallAsFunction(
    _ ctx: JSContextRef!,
    _ object: JSObjectRef!,
    _ thisObject: JSObjectRef!,
    _ argumentCount: Int,
    _ arguments: UnsafePointer!,
    _ exception: UnsafeMutablePointer!
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef to call as a function.

`thisObject`  

The object to use as `this`, or `NULL` to use the global object as `this`.

`argumentCount`  

An integer count of the number of arguments in `arguments`.

`arguments`  

A JSValueRef array of arguments to pass to the function. Pass `NULL` if `argumentCount` is `0`.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

The JSValueRef that results from calling `object` as a function, or `NULL` if the system throws an exception or `object` isn’t a function.

## See Also

### Working with Objects

func JSObjectCallAsConstructor(JSContextRef!, JSObjectRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Calls an object as a constructor.

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

