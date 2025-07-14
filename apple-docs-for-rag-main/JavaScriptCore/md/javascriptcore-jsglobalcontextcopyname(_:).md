

- JavaScriptCore
-  JSGlobalContextCopyName(\_:) 

Function

# JSGlobalContextCopyName(\_:)

Gets a copy of the name of a context.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextCopyName(_ ctx: JSGlobalContextRef!) -> JSStringRef!
```

## Parameters 

`ctx`  

The JSGlobalContextRef with the name you want to get.

## Return Value

The name for `ctx`.

## Discussion

JavaScriptCore exposes the name of JSGlobalContextRef for remote debugging to make it easier to identify the context you want to attach to.

## See Also

### Managing the context’s name

func JSGlobalContextSetName(JSGlobalContextRef!, JSStringRef!)

Sets the remote debugging name for a context.

