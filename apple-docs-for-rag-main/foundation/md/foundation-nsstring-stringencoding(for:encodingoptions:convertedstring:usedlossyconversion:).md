

- Foundation
- NSString
-  stringEncoding(for:encodingOptions:convertedString:usedLossyConversion:) 

Type Method

# stringEncoding(for:encodingOptions:convertedString:usedLossyConversion:)

Returns the string encoding for the given data as detected by attempting to create a string according to the specified encoding options.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func stringEncoding(
    for data: Data,
    encodingOptions opts: [StringEncodingDetectionOptionsKey : Any]? = nil,
    convertedString string: AutoreleasingUnsafeMutablePointer?,
    usedLossyConversion: UnsafeMutablePointer?
) -> UInt
```

## Parameters 

`data`  

An `NSData` object containing bytes in an encoding to be determined.

`opts`  

Options to use when attempting to determine the string encoding. See `String Encoding Detection Options` for a full list of supported options.

`string`  

If a string encoding could be determined, upon return contains an `NSString` object constructed from data using the determined string encoding.

`usedLossyConversion`  

If a string encoding could be determined, upon return contains a `BOOL` value corresponding to whether lossy conversion was used.

## Return Value

An `NSStringEncoding` value, or `0` if a string encoding could not be determined.

## See Also

### Working with Encodings

class var availableStringEncodings: UnsafePointer&lt;UInt>

Returns a zero-terminated list of the encodings string objects support in the application’s environment.

class var defaultCStringEncoding: UInt

Returns the C-string encoding assumed for any method accepting a C string as an argument.

class func localizedName(of: UInt) -> String

Returns a human-readable string giving the name of a given encoding.

func canBeConverted(to: UInt) -> Bool

Returns a Boolean value that indicates whether the receiver can be converted to a given encoding without loss of information.

func data(using: UInt) -> Data?

Returns an `NSData` object containing a representation of the receiver encoded using a given encoding.

func data(using: UInt, allowLossyConversion: Bool) -> Data?

Returns an `NSData` object containing a representation of the receiver encoded using a given encoding.

var description: String

var fastestEncoding: UInt

The fastest encoding to which the receiver may be converted without loss of information.

var smallestEncoding: UInt

The smallest encoding to which the receiver can be converted without loss of information.

struct StringEncodingDetectionOptionsKey

NSString Handling Exception Names

These constants define the names of exceptions raised if `NSString` cannot represent a string in a given encoding, or parse a string as a property list.

