

- JavaScriptCore
-  JSGlobalContextIsInspectable(\_:) 

Function

# JSGlobalContextIsInspectable(\_:)

Returns a Boolean value that indicates whether the JavaScript context is inspectable.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextIsInspectable(_ ctx: JSGlobalContextRef!) -> Bool
```

## Parameters 

`ctx`  

The JSGlobalContextRef to check whether it’s inspectable.

## Return Value

A Boolean value that indicates whether the JavaScript context is inspectable.

## Topics

### Related Documentation

func JSGlobalContextCopyName(JSGlobalContextRef!) -> JSStringRef!

Gets a copy of the name of a context.

func JSGlobalContextSetName(JSGlobalContextRef!, JSStringRef!)

Sets the remote debugging name for a context.

## See Also

### Making a context inspectable

func JSGlobalContextSetInspectable(JSGlobalContextRef!, Bool)

Sets a JavaScript context to be either inspectable or not inspectable.

