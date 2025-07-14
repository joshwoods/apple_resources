

- JavaScriptCore
-  JSStringCopyCFString(\_:\_:) 

Function

# JSStringCopyCFString(\_:\_:)

Creates a Core Foundation string from a JavaScript string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringCopyCFString(
    _ alloc: CFAllocator!,
    _ string: JSStringRef!
) -> CFString!
```

## Parameters 

`alloc`  

The `alloc` parameter to pass to `CFStringCreate`.

`string`  

The JSStringRef to copy into the new CFString.

## Return Value

A CFString that contains `string`. Ownership follows The Create Rule.

## See Also

### Converting to and from Core Foundation Strings

func JSStringCreateWithCFString(CFString!) -> JSStringRef!

Creates a JavaScript string from a Core Foundation string.

