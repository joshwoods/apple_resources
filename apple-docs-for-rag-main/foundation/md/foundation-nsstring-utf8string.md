

- Foundation
- NSString
-  utf8String 

Instance Property

# utf8String

A null-terminated UTF8 representation of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var utf8String: UnsafePointer? { get }
```

## Discussion

This C string is a pointer to a structure inside the string object, which may have a lifetime shorter than the string object and will certainly not have a longer lifetime. Therefore, you should copy the C string if it needs to be stored outside of the memory context in which you use this property.

## See Also

### Getting C Strings

func cString(using: UInt) -> UnsafePointer&lt;CChar>?

Returns a representation of the string as a C string using a given encoding.

func getCString(UnsafeMutablePointer&lt;CChar>, maxLength: Int, encoding: UInt) -> Bool

Converts the string to a given encoding and stores it in a buffer.

