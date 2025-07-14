

- Foundation
- NSString
-  init(CString:) Deprecated

Initializer

# init(CString:)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
convenience init?(CString bytes: UnsafePointer)
```

``` source
convenience init?(cString bytes: UnsafePointer)
```

Deprecated

Use init(CString:encoding:) instead.

## Discussion

`cString` must be a zero-terminated C string in the default C string encoding, and may not be `NULL`. Returns an initialized object, which might be different from the original receiver.

To create an immutable string from an immutable C string buffer, do not attempt to use this method. Instead, use init(CStringNoCopy:length:freeWhenDone:).

## See Also

### Related Documentation

convenience init?(CString: UnsafePointer&lt;CChar>, encoding: UInt)

Returns an `NSString` object initialized using the characters in a given C array, interpreted according to a given encoding.

### Deprecated

class func string(withCString: UnsafePointer&lt;CChar>) -> Any?

Creates a new string using a given C-string.

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

func cStringLength() -> Int

Returns the length in char-sized units of the receiver’s C-string representation in the default C-string encoding.

Deprecated

func getCString(UnsafeMutablePointer&lt;CChar>)

Invokes getCString(_:maxLength:range:remaining:) with `NSMaximumStringLength` as the maximum length, the receiver’s entire extent as the range, and `NULL` for the remaining range.

Deprecated

