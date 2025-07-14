

- JavaScriptCore
-  JSGlobalContextRelease(\_:) 

Function

# JSGlobalContextRelease(\_:)

Releases a global JavaScript execution context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextRelease(_ ctx: JSGlobalContextRef!)
```

## Parameters 

`ctx`  

The JSGlobalContextRef to release.

## See Also

### Creating a global context

func JSGlobalContextCreate(JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context.

func JSGlobalContextCreateInGroup(JSContextGroupRef!, JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context in the provided context group.

func JSGlobalContextRetain(JSGlobalContextRef!) -> JSGlobalContextRef!

Retains a global JavaScript execution context.

