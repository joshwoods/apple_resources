

- JavaScriptCore
-  JSGlobalContextSetInspectable(\_:\_:) 

Function

# JSGlobalContextSetInspectable(\_:\_:)

Sets a JavaScript context to be either inspectable or not inspectable.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextSetInspectable(
    _ ctx: JSGlobalContextRef!,
    _ inspectable: Bool
)
```

## Parameters 

`ctx`  

The JSGlobalContextRef to set whether it’s inspectable.

`inspectable`  

A Boolean value that indicates whether the context is inspectable.

## Topics

### Related Documentation

func JSGlobalContextCopyName(JSGlobalContextRef!) -> JSStringRef!

Gets a copy of the name of a context.

func JSGlobalContextSetName(JSGlobalContextRef!, JSStringRef!)

Sets the remote debugging name for a context.

## See Also

### Making a context inspectable

func JSGlobalContextIsInspectable(JSGlobalContextRef!) -> Bool

Returns a Boolean value that indicates whether the JavaScript context is inspectable.

