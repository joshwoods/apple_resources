

- JavaScriptCore
-  JSGlobalContextCreate(\_:) 

Function

# JSGlobalContextCreate(\_:)

Creates a global JavaScript execution context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextCreate(_ globalObjectClass: JSClassRef!) -> JSGlobalContextRef!
```

## Parameters 

`globalObjectClass`  

The class to use when creating the global object. Pass `NULL` to use the default object class.

## Return Value

A JSGlobalContextRef with a global object of class `globalObjectClass`.

## Discussion

JSGlobalContextCreate(_:) allocates a global object and populates it with all the built-in JavaScript objects, such as `Object`, `Function`, `String`, and `Array`.

In WebKit 4 and later, the system creates the context in a unique context group. Therefore, scripts may execute in it concurrently with scripts executing in other contexts. However, you may not use values from the context in other contexts.

## See Also

### Creating a global context

func JSGlobalContextCreateInGroup(JSContextGroupRef!, JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context in the provided context group.

func JSGlobalContextRetain(JSGlobalContextRef!) -> JSGlobalContextRef!

Retains a global JavaScript execution context.

func JSGlobalContextRelease(JSGlobalContextRef!)

Releases a global JavaScript execution context.

