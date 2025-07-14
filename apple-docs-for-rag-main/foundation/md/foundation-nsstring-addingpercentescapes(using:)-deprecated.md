

- Foundation
- NSString
-  addingPercentEscapes(using:) Deprecated

Instance Method

# addingPercentEscapes(using:)

Returns a representation of the receiver using a given encoding to determine the percent escapes necessary to convert the receiver into a legal URL string.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func addingPercentEscapes(using enc: UInt) -> String?
```

Deprecated

Use addingPercentEncoding(withAllowedCharacters:) instead.

## Parameters 

`enc`  

The encoding to use for the returned string. If you are uncertain of the correct encoding you should use NSUTF8StringEncoding.

## Return Value

A representation of the receiver using `encoding` to determine the percent escapes necessary to convert the receiver into a legal URL string. Returns `nil` if `encoding` cannot encode a particular character.

## Discussion

It may be difficult to use this function to “clean up” unescaped or partially escaped URL strings where sequences are unpredictable. See CFURLCreateStringByAddingPercentEscapes(_:_:_:_:_:) for more information.

## See Also

### Related Documentation

func addingPercentEncoding(withAllowedCharacters: CharacterSet) -> String?

Returns a new string made from the receiver by replacing all characters not in the specified set with percent-encoded characters.

var removingPercentEncoding: String?

Returns a new string made from the receiver by replacing all percent encoded sequences with the matching UTF-8 characters.

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

func cStringLength() -> Int

Returns the length in char-sized units of the receiver’s C-string representation in the default C-string encoding.

Deprecated

