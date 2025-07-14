

- JavaScriptCore
-  JSValueProtect(\_:\_:) 

Function

# JSValueProtect(\_:\_:)

Protects a JavaScript value from garbage collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueProtect(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!
)
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to protect.

## Discussion

Use this method when you want to store a JSValueRef in a global or on the heap, where the garbage collector can’t discover your reference to it.

You can protect a value multiple times and must unprotect it an equal number of times before it becomes eligible for garbage collection.

## See Also

### Supporting Garbage Collection

func JSValueUnprotect(JSContextRef!, JSValueRef!)

Unprotects a JavaScript value from garbage collection.

