

- JavaScriptCore
-  JSGlobalContextSetName(\_:\_:) 

Function

# JSGlobalContextSetName(\_:\_:)

Sets the remote debugging name for a context.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextSetName(
    _ ctx: JSGlobalContextRef!,
    _ name: JSStringRef!
)
```

## Parameters 

`ctx`  

The JSGlobalContextRef that you want to name.

`name`  

The remote debugging name to set on `ctx`.

## See Also

### Managing the context’s name

func JSGlobalContextCopyName(JSGlobalContextRef!) -> JSStringRef!

Gets a copy of the name of a context.

