

- JavaScriptCore
-  JSStringIsEqualToUTF8CString(\_:\_:) 

Function

# JSStringIsEqualToUTF8CString(\_:\_:)

Tests whether a JavaScript string matches a null-terminated UTF-8 string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringIsEqualToUTF8CString(
    _ a: JSStringRef!,
    _ b: UnsafePointer!
) -> Bool
```

## Parameters 

`a`  

The JSStringRef to test.

`b`  

The null-terminated UTF-8 string to test.

## Return Value

true if the two strings match; otherwise, false.

## See Also

### Comparing JavaScript Strings

func JSStringIsEqual(JSStringRef!, JSStringRef!) -> Bool

Tests whether two JavaScript strings match.

