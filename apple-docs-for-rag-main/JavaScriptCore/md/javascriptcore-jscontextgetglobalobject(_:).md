

- JavaScriptCore
-  JSContextGetGlobalObject(\_:) 

Function

# JSContextGetGlobalObject(\_:)

Gets the global object of a JavaScript execution context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGetGlobalObject(_ ctx: JSContextRef!) -> JSObjectRef!
```

## Parameters 

`ctx`  

The JSContextRef with the global object you want to get.

## Return Value

The global object of `ctx`.

