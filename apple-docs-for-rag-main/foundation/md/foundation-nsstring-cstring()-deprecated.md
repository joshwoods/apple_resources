

- Foundation
- NSString
-  cString() Deprecated

Instance Method

# cString()

Returns a representation of the receiver as a C string in the default C-string encoding.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func cString() -> UnsafePointer?
```

Deprecated

Use cString(using:) or utf8String instead.

## Discussion

The returned C string will be automatically freed just as a returned object would be released; your code should copy the C string or use getCString(_:) if it needs to store the C string outside of the autorelease context in which the C string is created.

Raises an `NSCharacterConversionException` if the receiver can’t be represented in the default C-string encoding without loss of information. Use canBeConverted(to:) if necessary to check whether a string can be losslessly converted to the default C-string encoding. If it can’t, use lossyCString() or data(using:allowLossyConversion:) to get a C-string representation with some loss of information.

## See Also

### Related Documentation

func cString(using: UInt) -> UnsafePointer&lt;CChar>?

Returns a representation of the string as a C string using a given encoding.

var utf8String: UnsafePointer&lt;CChar>?

A null-terminated UTF8 representation of the string.

func getCString(UnsafeMutablePointer&lt;CChar>, maxLength: Int, encoding: UInt) -> Bool

Converts the string to a given encoding and stores it in a buffer.

### Deprecated

class func string(withCString: UnsafePointer&lt;CChar>) -> Any?

Creates a new string using a given C-string.

Deprecated

convenience init?(CString: UnsafePointer&lt;CChar>)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

class func string(withCString: UnsafePointer&lt;CChar>, length: Int) -> Any?

Returns a string containing the characters in a given C-string.

Deprecated

convenience init?(CString: UnsafePointer&lt;CChar>, length: Int)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

convenience init?(CStringNoCopy: UnsafeMutablePointer&lt;CChar>, length: Int, freeWhenDone: Bool)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

class func string(withContentsOfFile: String) -> Any?

Returns a string created by reading data from the file named by a given path.

Deprecated

convenience init?(contentsOfFile: String)

Initializes the receiver, a newly allocated `NSString` object, by reading data from the file named by `path`.

Deprecated

class func string(withContentsOf: URL) -> Any?

Returns a string created by reading data from the file named by a given URL.

Deprecated

convenience init?(contentsOfURL: URL)

Initializes the receiver, a newly allocated `NSString` object, by reading data from the location named by a given URL.

Deprecated

func write(toFile: String, atomically: Bool) -> Bool

Writes the contents of the receiver to the file specified by a given path.

Deprecated

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the receiver to the location specified by a given URL.

Deprecated

func getCharacters(UnsafeMutablePointer&lt;unichar>)

Copies all characters from the receiver into a given buffer.

Deprecated

func lossyCString() -> UnsafePointer&lt;CChar>?

Returns a representation of the receiver as a C string in the default C-string encoding, possibly losing information in converting to that encoding.

Deprecated

func cStringLength() -> Int

Returns the length in char-sized units of the receiver’s C-string representation in the default C-string encoding.

Deprecated

func getCString(UnsafeMutablePointer&lt;CChar>)

Invokes getCString(_:maxLength:range:remaining:) with `NSMaximumStringLength` as the maximum length, the receiver’s entire extent as the range, and `NULL` for the remaining range.

Deprecated

