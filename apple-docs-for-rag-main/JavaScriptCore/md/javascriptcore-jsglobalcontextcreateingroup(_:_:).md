

- JavaScriptCore
-  JSGlobalContextCreateInGroup(\_:\_:) 

Function

# JSGlobalContextCreateInGroup(\_:\_:)

Creates a global JavaScript execution context in the provided context group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextCreateInGroup(
    _ group: JSContextGroupRef!,
    _ globalObjectClass: JSClassRef!
) -> JSGlobalContextRef!
```

## Parameters 

`group`  

The context group to use. The created global context retains the group. Pass `NULL` to create a unique group for the context.

`globalObjectClass`  

The class to use when creating the global object. Pass `NULL` to use the default object class.

## Return Value

A JSGlobalContextRef with a global object of class `globalObjectClass` and a context group equal to `group`.

## Discussion

JSGlobalContextCreateInGroup(_:_:) allocates a global object and populates it with all the built-in JavaScript objects, such as `Object`, `Function`, `String`, and `Array`.

## See Also

### Creating a global context

func JSGlobalContextCreate(JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context.

func JSGlobalContextRetain(JSGlobalContextRef!) -> JSGlobalContextRef!

Retains a global JavaScript execution context.

func JSGlobalContextRelease(JSGlobalContextRef!)

Releases a global JavaScript execution context.

