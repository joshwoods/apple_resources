

- Foundation
- NSString
-  init(CString:encoding:) 

Initializer

# init(CString:encoding:)

Returns an `NSString` object initialized using the characters in a given C array, interpreted according to a given encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(
    CString nullTerminatedCString: UnsafePointer,
    encoding: UInt
)
```

``` source
convenience init?(
    cString nullTerminatedCString: UnsafePointer,
    encoding: UInt
)
```

## Parameters 

`nullTerminatedCString`  

A C array of characters. The array must end with a `NULL` character; intermediate `NULL` characters are not allowed.

`encoding`  

The encoding of `nullTerminatedCString`. For possible values, see NSStringEncoding.

## Return Value

An `NSString` object initialized using the characters from `nullTerminatedCString`. The returned object may be different from the original receiver

## Discussion

If `nullTerminatedCString` is not a `NULL`-terminated C string, or `encoding` does not match the actual character encoding, the results are undefined.

### Special Considerations

Only 8-bit encodings are supported, as encodings that have a greater width, such as UTF-16, may include a `NULL` byte in a single unit, which would result in the premature termination of the C string.

## See Also

### Related Documentation

class func string(withCString: UnsafePointer&lt;CChar>) -> Any?

Creates a new string using a given C-string.

Deprecated

convenience init?(CStringNoCopy: UnsafeMutablePointer&lt;CChar>, length: Int, freeWhenDone: Bool)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

class var defaultCStringEncoding: UInt

Returns the C-string encoding assumed for any method accepting a C string as an argument.

### Creating and Initializing Strings

init()

Returns an initialized `NSString` object that contains no characters.

convenience init?(bytes: UnsafeRawPointer, length: Int, encoding: UInt)

Returns an initialized `NSString` object containing a given number of bytes from a given buffer of bytes interpreted in a given encoding.

convenience init?(bytesNoCopy: UnsafeMutableRawPointer, length: Int, encoding: UInt, freeWhenDone: Bool)

Returns an initialized `NSString` object that contains a given number of bytes from a given buffer of bytes interpreted in a given encoding, and optionally frees the buffer.

convenience init(characters: UnsafePointer&lt;unichar>, length: Int)

Returns an initialized `NSString` object that contains a given number of characters from a given C array of UTF-16 code units.

convenience init(charactersNoCopy: UnsafeMutablePointer&lt;unichar>, length: Int, freeWhenDone: Bool)

Returns an initialized `NSString` object that contains a given number of characters from a given C array of UTF-16 code units.

convenience init(string: String)

Returns an `NSString` object initialized by copying the characters from another given string.

convenience init?(UTF8String: UnsafePointer&lt;CChar>)

Returns an `NSString` object initialized by copying the characters from a given C array of UTF8-encoded bytes.

convenience init(format: String, arguments: CVaListPointer)

Returns an `NSString` object initialized by using a given format string as a template into which the remaining argument values are substituted without any localization.

convenience init(format: String, locale: Any?, arguments: CVaListPointer)

Returns an `NSString` object initialized by using a given format string as a template into which the remaining argument values are substituted according to given locale information. This method is meant to be called from within a variadic function, where the argument list will be available.

convenience init?(data: Data, encoding: UInt)

Returns an `NSString` object initialized by converting given data into UTF-16 code units using a given encoding.

class func localizedUserNotificationString(forKey: String, arguments: [Any]?) -> String

Returns a localized string intended for display in a notification alert.

class func localizedStringWithFormat(NSString, any CVarArg...) -> Self

convenience init?(CString: UnsafePointer&lt;CChar>, encoding: UInt)

Returns a string containing the bytes in a given C array, interpreted according to a given encoding.

convenience init?(UTF8String: UnsafePointer&lt;CChar>)

Returns a string created by copying the data from a given C array of UTF8-encoded bytes.

typealias unichar

Type for UTF-16 code units.

