

- JavaScriptCore
-  JSValueUnprotect(\_:\_:) 

Function

# JSValueUnprotect(\_:\_:)

Unprotects a JavaScript value from garbage collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueUnprotect(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!
)
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to unprotect.

## Discussion

You can protect a value multiple times and must unprotect it an equal number of times before it becomes eligible for garbage collection.

## See Also

### Supporting Garbage Collection

func JSValueProtect(JSContextRef!, JSValueRef!)

Protects a JavaScript value from garbage collection.

