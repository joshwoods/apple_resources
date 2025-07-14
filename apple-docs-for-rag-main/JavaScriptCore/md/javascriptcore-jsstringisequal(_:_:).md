

- JavaScriptCore
-  JSStringIsEqual(\_:\_:) 

Function

# JSStringIsEqual(\_:\_:)

Tests whether two JavaScript strings match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringIsEqual(
    _ a: JSStringRef!,
    _ b: JSStringRef!
) -> Bool
```

## Parameters 

`a`  

The first JSStringRef to test.

`b`  

The second JSStringRef to test.

## Return Value

true if the two strings match; otherwise, false.

## See Also

### Comparing JavaScript Strings

func JSStringIsEqualToUTF8CString(JSStringRef!, UnsafePointer&lt;CChar>!) -> Bool

Tests whether a JavaScript string matches a null-terminated UTF-8 string.

