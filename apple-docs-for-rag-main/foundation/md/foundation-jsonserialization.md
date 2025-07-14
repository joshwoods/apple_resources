

- Foundation
-  JSONSerialization 

Class

# JSONSerialization

An object that converts between JSON and the equivalent Foundation objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class JSONSerialization
```

## Overview

You use the JSONSerialization class to convert JSON to Foundation objects and convert Foundation objects to JSON.

To convert a Foundation object to JSON, the object must have the following properties:

- The top level object is an NSArray or NSDictionary, unless you set the fragmentsAllowed option.

- All objects are instances of NSString, NSNumber, NSArray, NSDictionary, or NSNull.

- All dictionary keys are instances of NSString.

- Numbers are neither `NaN` nor infinity.

Other rules may apply. Calling isValidJSONObject(_:) or attempting a conversion are the definitive ways to tell if the JSONSerialization class can convert given object to JSON data.

Note

On iOS 7 and later and macOS 10.9 and later, JSONSerialization is thread safe.

## Topics

### Creating a JSON Object

class func jsonObject(with: Data, options: JSONSerialization.ReadingOptions) throws -> Any

Returns a Foundation object from given JSON data.

class func jsonObject(with: InputStream, options: JSONSerialization.ReadingOptions) throws -> Any

Returns a Foundation object from JSON data in a given stream.

struct ReadingOptions

Options used when creating Foundation objects from JSON data.

### Creating JSON Data

class func data(withJSONObject: Any, options: JSONSerialization.WritingOptions) throws -> Data

Returns JSON data from a Foundation object.

class func writeJSONObject(Any, to: OutputStream, options: JSONSerialization.WritingOptions, error: NSErrorPointer) -> Int

Writes a given JSON object to a stream.

struct WritingOptions

Options for writing JSON data.

class func isValidJSONObject(Any) -> Bool

Returns a Boolean value that indicates whether the serializer can convert a given object to JSON data.

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

### JSON

class JSONEncoder

An object that encodes instances of a data type as JSON objects.

class JSONDecoder

An object that decodes instances of a data type from JSON objects.

