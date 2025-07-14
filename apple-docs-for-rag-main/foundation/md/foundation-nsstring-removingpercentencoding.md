

- Foundation
- NSString
-  removingPercentEncoding 

Instance Property

# removingPercentEncoding

Returns a new string made from the receiver by replacing all percent encoded sequences with the matching UTF-8 characters.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var removingPercentEncoding: String? { get }
```

## Return Value

A new string with the percent-encoded sequences removed, or `nil` if the receiver contains an invalid percent-encoding sequence.

## Discussion

Important

You must call this method only on strings that you know to be percent-encoded. Calling this method on strings that are not percent-encoded can lead to misinterpreting a percent character as the beginning of a percent-encoded sequence.

## See Also

### Related Documentation

func replacingPercentEscapes(using: UInt) -> String?

Returns a new string made by replacing in the receiver all percent escapes with the matching characters as determined by a given encoding.

Deprecated

func addingPercentEscapes(using: UInt) -> String?

Returns a representation of the receiver using a given encoding to determine the percent escapes necessary to convert the receiver into a legal URL string.

Deprecated

### Working with URL Strings

func addingPercentEncoding(withAllowedCharacters: CharacterSet) -> String?

Returns a new string made from the receiver by replacing all characters not in the specified set with percent-encoded characters.

