

- Foundation
- NSString
-  init(CStringNoCopy:length:freeWhenDone:) Deprecated

Initializer

# init(CStringNoCopy:length:freeWhenDone:)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
convenience init?(
    CStringNoCopy bytes: UnsafeMutablePointer,
    length: Int,
    freeWhenDone freeBuffer: Bool
)
```

``` source
convenience init?(
    cStringNoCopy bytes: UnsafeMutablePointer,
    length: Int,
    freeWhenDone freeBuffer: Bool
)
```

Deprecated

Use init(bytesNoCopy:length:encoding:freeWhenDone:) instead.

## Discussion

This method converts `length` \* `sizeof(char)` bytes from `cString` and doesn’t stop short at a zero character. `cString` must contain data in the default C-string encoding and may not be `NULL`. The receiver becomes the owner of `cString`; if `flag` is true it will free the memory when it no longer needs it, but if `flag` is false it won’t. Returns an initialized object, which might be different from the original receiver.

You can use this method to create an immutable string from an immutable (`const char *`) C-string buffer. If you receive a warning message, you can disregard it; its purpose is simply to warn you that the C string passed as the method’s first argument may be modified. If you make certain the `freeWhenDone` argument to `initWithStringNoCopy` is false, the C string passed as the method’s first argument cannot be modified, so you can safely use `initWithStringNoCopy` to create an immutable string from an immutable (`const char *`) C-string buffer.

## See Also

### Related Documentation

convenience init?(CString: UnsafePointer&lt;CChar>, encoding: UInt)

Returns an `NSString` object initialized using the characters in a given C array, interpreted according to a given encoding.

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

