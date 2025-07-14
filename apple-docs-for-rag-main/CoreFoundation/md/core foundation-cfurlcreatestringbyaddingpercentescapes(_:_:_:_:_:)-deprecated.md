

- Core Foundation
-  CFURLCreateStringByAddingPercentEscapes(\_:\_:\_:\_:\_:) Deprecated

Function

# CFURLCreateStringByAddingPercentEscapes(\_:\_:\_:\_:\_:)

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLCreateStringByAddingPercentEscapes(
    _ allocator: CFAllocator!,
    _ originalString: CFString!,
    _ charactersToLeaveUnescaped: CFString!,
    _ legalURLCharactersToBeEscaped: CFString!,
    _ encoding: CFStringEncoding
) -> CFString!
```

Deprecated

Use \[NSString stringByAddingPercentEncodingWithAllowedCharacters:\] instead, which always uses the recommended UTF-8 encoding, and which encodes for a specific URL component or subcomponent (since each URL component or subcomponent has different rules for what characters are valid).

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFString` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`originalString`  

The `CFString` object to copy.

`charactersToLeaveUnescaped`  

Characters whose percent escape sequences you want to leave intact. Pass `NULL` to specify that all illegal characters be escaped.

`legalURLCharactersToBeEscaped`  

Legal characters to be escaped. Pass `NULL` to specify that no legal characters be replaced.

`encoding`  

The encoding to use for the translation. If you are uncertain of the correct encoding, you should use UTF-8 (CFStringBuiltInEncodings.UTF8), which is the encoding designated by RFC 2396 as the correct encoding for use in URLs.

## Return Value

A copy of `originalString` replacing certain characters. If it does not need to be modified (no percent escape sequences are missing), this function may merely return `originalString` with its reference count incremented. Ownership follows the create rule. See The Create Rule.

## Discussion

The characters escaped are all characters that are not legal URL characters (based on RFC 2396), plus any characters in `legalURLCharactersToBeEscaped`, less any characters in `charactersToLeaveUnescaped`. To simply correct any non-URL characters in an otherwise correct URL string, pass `NULL` for the `allocator`, `charactersToLeaveEscaped`, and `legalURLCharactersToBeEscaped` parameters, and CFStringBuiltInEncodings.UTF8 as the `encoding` parameter.

It may be difficult to use this function to “clean up” unescaped or partially escaped URL strings where sequences are unpredictable and you cannot specify `charactersToLeaveUnescaped`. Instead, you can “pre-process” a URL string using CFURLCreateStringByReplacingPercentEscapesUsingEncoding(_:_:_:_:) then add the escape characters using CFURLCreateStringByAddingPercentEscapes(_:_:_:_:_:), as shown in the following code fragment.

```
CFStringRef originalURLString = CFSTR("http://online.store.com/storefront/?request=get-document&doi=10.1175%2F1520-0426(2005)014%3C1157:DODADSS%3E2.0.CO%3B2");
CFStringRef preprocessedString =
    CFURLCreateStringByReplacingPercentEscapesUsingEncoding(kCFAllocatorDefault, originalURLString, CFSTR(""), kCFStringEncodingUTF8);
CFStringRef urlString =
    CFURLCreateStringByAddingPercentEscapes(kCFAllocatorDefault, preprocessedString, NULL, NULL, kCFStringEncodingUTF8);
url = CFURLCreateWithString(kCFAllocatorDefault, urlString, NULL);
```

## See Also

### Converting URLs to Other Representations

func CFURLCreateData(CFAllocator!, CFURL!, CFStringEncoding, Bool) -> CFData!

Creates a `CFData` object containing the content of a given URL.

func CFURLCreateStringByReplacingPercentEscapes(CFAllocator!, CFString!, CFString!) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

func CFURLCreateStringByReplacingPercentEscapesUsingEncoding(CFAllocator!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

Deprecated

func CFURLGetFileSystemRepresentation(CFURL!, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> Bool

Fills a buffer with the file system’s native string representation of a given URL’s path.

func CFURLGetFSRef(CFURL!, OpaquePointer!) -> Bool

Converts a given URL to a file or directory object.

Deprecated

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

