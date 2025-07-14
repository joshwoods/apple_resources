

- Foundation
- NSString
-  defaultCStringEncoding 

Type Property

# defaultCStringEncoding

Returns the C-string encoding assumed for any method accepting a C string as an argument.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var defaultCStringEncoding: UInt { get }
```

## Return Value

The C-string encoding assumed for any method accepting a C string as an argument.

## Discussion

This method returns a user-dependent encoding who value is derived from user’s default language and potentially other factors. You might sometimes need to use this encoding when interpreting user documents with unknown encodings, in the absence of other hints, but in general this encoding should be used rarely, if at all. Note that some potential values might result in unexpected encoding conversions of even fairly straightforward `NSString` content—for example, punctuation characters with a bidirectional encoding.

Methods that accept a C string as an argument use `...CString...` in the keywords for such arguments: for example, string(withCString:)—note, though, that these are deprecated. The default C-string encoding is determined from system information and can’t be changed programmatically for an individual process. See NSStringEncoding for a full list of supported encodings.

## See Also

### Working with Encodings

class var availableStringEncodings: UnsafePointer&lt;UInt>

Returns a zero-terminated list of the encodings string objects support in the application’s environment.

class func stringEncoding(for: Data, encodingOptions: [StringEncodingDetectionOptionsKey : Any]?, convertedString: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, usedLossyConversion: UnsafeMutablePointer&lt;ObjCBool>?) -> UInt

Returns the string encoding for the given data as detected by attempting to create a string according to the specified encoding options.

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

