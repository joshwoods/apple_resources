

- Foundation
- NSString
-  init(UTF8String:) 

Initializer

# init(UTF8String:)

Returns an `NSString` object initialized by copying the characters from a given C array of UTF8-encoded bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(UTF8String nullTerminatedCString: UnsafePointer)
```

``` source
convenience init?(utf8String nullTerminatedCString: UnsafePointer)
```

## Parameters 

`nullTerminatedCString`  

A `NULL`-terminated C array of bytes in UTF-8 encoding. This value must not be `NULL`.

Important

Raises an exception if `nullTerminatedCString` is `NULL`.

## Return Value

An `NSString` object initialized by copying the bytes from `nullTerminatedCString`. The returned object may be different from the original receiver.

## See Also

### Related Documentation

convenience init?(UTF8String: UnsafePointer&lt;CChar>)

Returns a string created by copying the data from a given C array of UTF8-encoded bytes.

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

convenience init?(CString: UnsafePointer&lt;CChar>, encoding: UInt)

Returns an `NSString` object initialized using the characters in a given C array, interpreted according to a given encoding.

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

