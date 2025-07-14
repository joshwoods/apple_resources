

- Foundation
- NSString
-  canBeConverted(to:) 

Instance Method

# canBeConverted(to:)

Returns a Boolean value that indicates whether the receiver can be converted to a given encoding without loss of information.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func canBeConverted(to encoding: UInt) -> Bool
```

## Parameters 

`encoding`  

A string encoding. For possible values, see NSStringEncoding.

## Return Value

true if the receiver can be converted to `encoding` without loss of information. Returns false if characters would have to be changed or deleted in the process of changing encodings.

## Discussion

If you plan to actually convert a string, the `dataUsingEncoding:...` methods return `nil` on failure, so you can avoid the overhead of invoking this method yourself by simply trying to convert the string.

## See Also

### Working with Encodings

class var availableStringEncodings: UnsafePointer&lt;UInt>

Returns a zero-terminated list of the encodings string objects support in the application’s environment.

class var defaultCStringEncoding: UInt

Returns the C-string encoding assumed for any method accepting a C string as an argument.

class func stringEncoding(for: Data, encodingOptions: [StringEncodingDetectionOptionsKey : Any]?, convertedString: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, usedLossyConversion: UnsafeMutablePointer&lt;ObjCBool>?) -> UInt

Returns the string encoding for the given data as detected by attempting to create a string according to the specified encoding options.

class func localizedName(of: UInt) -> String

Returns a human-readable string giving the name of a given encoding.

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

