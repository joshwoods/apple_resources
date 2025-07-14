

- Foundation
-  PropertyListSerialization 

Class

# PropertyListSerialization

An object that converts between a property list and one of several serialized representations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class PropertyListSerialization
```

## Overview

The PropertyListSerialization class provides methods that convert a property list to and from several serialized formats. A property list is itself an array or dictionary that contains only NSData, NSString, NSArray, NSDictionary, NSDate, and NSNumber objects.

Property list objects are toll-free bridged with their respective Core Foundation types (CFData, CFString, and so on). See Toll-Free Bridging for more information on toll-free bridging.

## Topics

### Serializing a Property List

class func data(fromPropertyList: Any, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions) throws -> Data

Returns an `NSData` object containing a given property list in a specified format.

class func writePropertyList(Any, to: OutputStream, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions, error: NSErrorPointer) -> Int

Writes a property list to the specified stream.

typealias WriteOptions

### Deserializing a Property List

class func propertyList(from: Data, options: PropertyListSerialization.ReadOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?) throws -> Any

Creates and returns a property list from the specified data.

class func propertyList(with: InputStream, options: PropertyListSerialization.ReadOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?) throws -> Any

Creates and returns a property list by reading from the specified stream.

### Validating a Property List

class func propertyList(Any, isValidFor: PropertyListSerialization.PropertyListFormat) -> Bool

Returns a Boolean value that indicates whether a given property list is valid for a given format.

### Obsolete Methods

class func dataFromPropertyList(Any, format: PropertyListSerialization.PropertyListFormat, errorDescription: UnsafeMutablePointer&lt;NSString?>?) -> Data?

This method is obsolete and will be deprecated soon.

Deprecated

class func propertyListFromData(Data, mutabilityOption: PropertyListSerialization.MutabilityOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?, errorDescription: UnsafeMutablePointer&lt;NSString?>?) -> Any?

This method is deprecated. Use data(fromPropertyList:format:options:) instead.

Deprecated

### Constants

struct MutabilityOptions

These constants specify mutability options in property lists.

enum PropertyListFormat

These constants are used to specify a property list serialization format.

typealias ReadOptions

The only read options supported are described in PropertyListSerialization.MutabilityOptions.

### Error Codes

var NSPropertyListReadCorruptError: Int

Parsing of the property list failed.

var NSPropertyListReadUnknownVersionError: Int

The version number of the property list cannot be determined.

var NSPropertyListReadStreamError: Int

Reading of the property list failed.

var NSPropertyListWriteStreamError: Int

Writing to the property list failed.

var NSPropertyListWriteInvalidError: Int

Writing failed because of an invalid property list object, or an invalid property list type was specified.

var NSPropertyListErrorMinimum: Int

The start of the range of error codes reserved for property list errors.

var NSPropertyListErrorMaximum: Int

The end of the range of error codes reserved for property list errors.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Property Lists

class PropertyListEncoder

An object that encodes instances of data types to a property list.

class PropertyListDecoder

An object that decodes instances of data types from a property list.

