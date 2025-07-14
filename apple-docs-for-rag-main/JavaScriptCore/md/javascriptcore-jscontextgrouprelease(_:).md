

- JavaScriptCore
-  JSContextGroupRelease(\_:) 

Function

# JSContextGroupRelease(\_:)

Releases a JavaScript context group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGroupRelease(_ group: JSContextGroupRef!)
```

## Parameters 

`group`  

The JSContextGroupRef to release.

## See Also

### Creating a Context Group

func JSContextGroupCreate() -> JSContextGroupRef!

Creates a JavaScript context group.

func JSContextGroupRetain(JSContextGroupRef!) -> JSContextGroupRef!

Retains a JavaScript context group.

