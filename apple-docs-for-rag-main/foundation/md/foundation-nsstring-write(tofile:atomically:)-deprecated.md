

- Foundation
- NSString
-  write(toFile:atomically:) Deprecated

Instance Method

# write(toFile:atomically:)

Writes the contents of the receiver to the file specified by a given path.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func write(
    toFile path: String,
    atomically useAuxiliaryFile: Bool
) -> Bool
```

Deprecated

Use write(toFile:atomically:encoding:) instead.

## Return Value

true if the file is written successfully, otherwise false.

## Discussion

Writes the contents of the receiver to the file specified by `path` (overwriting any existing file at `path`). `path` is written in the default C-string encoding if possible (that is, if no information would be lost), in the Unicode encoding otherwise.

If `flag` is true, the receiver is written to an auxiliary file, and then the auxiliary file is renamed to `path`. If `flag` is false, the receiver is written directly to `path`. The true option guarantees that `path`, if it exists at all, won’t be corrupted even if the system should crash during writing.

If `path` contains a tilde (`~`) character, you must expand it with expandingTildeInPath before invoking this method.

## See Also

### Related Documentation

func write(toFile: String, atomically: Bool, encoding: UInt) throws

Writes the contents of the receiver to a file at a given path using a given encoding.

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

