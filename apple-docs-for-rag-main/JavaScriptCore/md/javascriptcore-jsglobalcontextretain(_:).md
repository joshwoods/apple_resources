

- JavaScriptCore
-  JSGlobalContextRetain(\_:) 

Function

# JSGlobalContextRetain(\_:)

Retains a global JavaScript execution context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSGlobalContextRetain(_ ctx: JSGlobalContextRef!) -> JSGlobalContextRef!
```

## Parameters 

`ctx`  

The JSGlobalContextRef to retain.

## Return Value

A JSGlobalContextRef that is the same as `ctx`.

## See Also

### Creating a global context

func JSGlobalContextCreate(JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context.

func JSGlobalContextCreateInGroup(JSContextGroupRef!, JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context in the provided context group.

func JSGlobalContextRelease(JSGlobalContextRef!)

Releases a global JavaScript execution context.

