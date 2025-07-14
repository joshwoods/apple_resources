

- Foundation
- NSString
-  addingPercentEncoding(withAllowedCharacters:) 

Instance Method

# addingPercentEncoding(withAllowedCharacters:)

Returns a new string made from the receiver by replacing all characters not in the specified set with percent-encoded characters.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addingPercentEncoding(withAllowedCharacters allowedCharacters: CharacterSet) -> String?
```

## Parameters 

`allowedCharacters`  

The characters not replaced in the string. Typically, you specify one of the predefined character sets for a particular URL component, such as urlPathAllowed or urlQueryAllowed.

## Return Value

Returns the encoded string, or `nil` if the transformation is not possible.

## Discussion

Entire URL strings cannot be percent-encoded, because each URL component specifies a different set of allowed characters. For example, the query component of a URL allows the “`@`” character, but that character must be percent-encoded in the password component.

UTF-8 encoding is used to determine the correct percent-encoded characters. Any characters in `allowedCharacters` outside of the 7-bit ASCII range are ignored.

Important

You must not call this method on strings that are already percent-encoded. Calling this method on strings that are already percent-encoded will cause percent characters in a percent-encoded sequence to be percent-encoded twice.

## See Also

### Related Documentation

func replacingPercentEscapes(using: UInt) -> String?

Returns a new string made by replacing in the receiver all percent escapes with the matching characters as determined by a given encoding.

Deprecated

func addingPercentEscapes(using: UInt) -> String?

Returns a representation of the receiver using a given encoding to determine the percent escapes necessary to convert the receiver into a legal URL string.

Deprecated

### Working with URL Strings

var removingPercentEncoding: String?

Returns a new string made from the receiver by replacing all percent encoded sequences with the matching UTF-8 characters.

