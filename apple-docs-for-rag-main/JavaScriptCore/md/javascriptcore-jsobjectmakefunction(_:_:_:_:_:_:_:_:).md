

- JavaScriptCore
-  JSObjectMakeFunction(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# JSObjectMakeFunction(\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a function with a specified script as its body.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectMakeFunction(
    _ ctx: JSContextRef!,
    _ name: JSStringRef!,
    _ parameterCount: UInt32,
    _ parameterNames: UnsafePointer!,
    _ body: JSStringRef!,
    _ sourceURL: JSStringRef!,
    _ startingLineNumber: Int32,
    _ exception: UnsafeMutablePointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`name`  

A JSStringRef that contains the function’s name. The system uses this when converting the function to a string. Pass `NULL` to create an anonymous function.

`parameterCount`  

An integer count of the number of parameter names in `parameterNames`.

`parameterNames`  

A JSStringRef array that contains the names of the function’s parameters. Pass `NULL` if `parameterCount` is `0`.

`body`  

A JSStringRef that contains the script to use as the function’s body.

`sourceURL`  

A JSStringRef that contains a URL for the script’s source file. The system only uses this when reporting exceptions. Pass `NULL` if you don’t want to include source file information in exceptions.

`startingLineNumber`  

An integer value that specifies the script’s starting line number in the file at `sourceURL`. The system only uses this when reporting exceptions.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A JSObjectRef that is a function, or `NULL` if either `body` or `parameterNames` contains a syntax error. The object’s prototype is the default function prototype.

## Discussion

Use this method when you want to execute a script repeatedly to avoid the cost of reparsing the script before each execution.

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

