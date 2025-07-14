

- JavaScriptCore
-  JSContextGetGlobalContext(\_:) 

Function

# JSContextGetGlobalContext(\_:)

Gets the global context of a JavaScript execution context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGetGlobalContext(_ ctx: JSContextRef!) -> JSGlobalContextRef!
```

## Parameters 

`ctx`  

The `JSContextRef` with the global context you want to get.

## Return Value

The global context of `ctx`.

