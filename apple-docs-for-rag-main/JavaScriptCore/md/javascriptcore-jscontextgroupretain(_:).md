

- JavaScriptCore
-  JSContextGroupRetain(\_:) 

Function

# JSContextGroupRetain(\_:)

Retains a JavaScript context group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGroupRetain(_ group: JSContextGroupRef!) -> JSContextGroupRef!
```

## Parameters 

`group`  

The JSContextGroupRef to retain.

## Return Value

A JSContextGroupRef that is the same as `group`.

## See Also

### Creating a Context Group

func JSContextGroupCreate() -> JSContextGroupRef!

Creates a JavaScript context group.

func JSContextGroupRelease(JSContextGroupRef!)

Releases a JavaScript context group.

