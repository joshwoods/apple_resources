

- Foundation
- NSString
-  cStringLength() Deprecated

Instance Method

# cStringLength()

Returns the length in char-sized units of the receiver’s C-string representation in the default C-string encoding.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func cStringLength() -> Int
```

Deprecated

Use lengthOfBytes(using:) or maximumLengthOfBytes(using:) instead.

## Discussion

Raises if the receiver can’t be represented in the default C-string encoding without loss of information. You can also use canBeConverted(to:) to check whether a string can be losslessly converted to the default C-string encoding. If it can’t, use lossyCString() to get a C-string representation with some loss of information, then check its length explicitly using the ANSI function `strlen()`.

## See Also

### Related Documentation

var utf8String: UnsafePointer&lt;CChar>?

A null-terminated UTF8 representation of the string.

func maximumLengthOfBytes(using: UInt) -> Int

Returns the maximum number of bytes needed to store the receiver in a given encoding.

func lengthOfBytes(using: UInt) -> Int

Returns the number of bytes required to store the receiver in a given encoding.

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

func cString() -> UnsafePointer&lt;CChar>?

Returns a representation of the receiver as a C string in the default C-string encoding.

Deprecated

func lossyCString() -> UnsafePointer&lt;CChar>?

Returns a representation of the receiver as a C string in the default C-string encoding, possibly losing information in converting to that encoding.

Deprecated

func getCString(UnsafeMutablePointer&lt;CChar>)

Invokes getCString(_:maxLength:range:remaining:) with `NSMaximumStringLength` as the maximum length, the receiver’s entire extent as the range, and `NULL` for the remaining range.

Deprecated

