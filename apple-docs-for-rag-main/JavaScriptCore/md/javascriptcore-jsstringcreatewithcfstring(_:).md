

- JavaScriptCore
-  JSStringCreateWithCFString(\_:) 

Function

# JSStringCreateWithCFString(\_:)

Creates a JavaScript string from a Core Foundation string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringCreateWithCFString(_ string: CFString!) -> JSStringRef!
```

## Parameters 

`string`  

The CFString to copy into the new JSStringRef.

## Return Value

A JSStringRef that contains `string`. Ownership follows The Create Rule.

## Discussion

The system optimizes this function to take advantage of cases when CFStringGetCharactersPtr(_:) returns a valid pointer.

## See Also

### Converting to and from Core Foundation Strings

func JSStringCopyCFString(CFAllocator!, JSStringRef!) -> CFString!

Creates a Core Foundation string from a JavaScript string.

