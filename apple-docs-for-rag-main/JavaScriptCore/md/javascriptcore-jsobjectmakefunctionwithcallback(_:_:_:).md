

- JavaScriptCore
-  JSObjectMakeFunctionWithCallback(\_:\_:\_:) 

Function

# JSObjectMakeFunctionWithCallback(\_:\_:\_:)

Creates a JavaScript function with a specified callback as its implementation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectMakeFunctionWithCallback(
    _ ctx: JSContextRef!,
    _ name: JSStringRef!,
    _ callAsFunction: JSObjectCallAsFunctionCallback!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`name`  

A JSStringRef that contains the function’s name. The system uses this when converting the function to a string. Pass `NULL` to create an anonymous function.

`callAsFunction`  

The JSObjectCallAsFunctionCallback to invoke when calling the function.

## Return Value

A JSObjectRef that is a function. The object’s prototype is the default function prototype.

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

func JSObjectMake(JSContextRef!, JSClassRef!, UnsafeMutableRawPointer!) -> JSObjectRef!

Creates a JavaScript object.

func JSObjectMakeArray(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array object.

func JSObjectMakeConstructor(JSContextRef!, JSClassRef!, JSObjectCallAsConstructorCallback!) -> JSObjectRef!

Creates a JavaScript constructor.

func JSObjectMakeDate(JSContextRef!, Int, UnsafePointer&lt;JSValueRef?>!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript date object as though invoking the built-in date constructor.

