

- JavaScriptCore
-  JSContextGetGroup(\_:) 

Function

# JSContextGetGroup(\_:)

Gets the context group that a JavaScript execution context belongs to.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGetGroup(_ ctx: JSContextRef!) -> JSContextGroupRef!
```

## Parameters 

`ctx`  

The JSContextRef with the group you want to get.

## Return Value

The group that `ctx` belongs to.

