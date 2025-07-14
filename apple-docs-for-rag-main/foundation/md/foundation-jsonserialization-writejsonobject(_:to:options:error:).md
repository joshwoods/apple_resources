

- Foundation
- JSONSerialization
-  writeJSONObject(\_:to:options:error:) 

Type Method

# writeJSONObject(\_:to:options:error:)

Writes a given JSON object to a stream.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func writeJSONObject(
    _ obj: Any,
    to stream: OutputStream,
    options opt: JSONSerialization.WritingOptions = [],
    error: NSErrorPointer
) -> Int
```

## Parameters 

`obj`  

The object to write to `stream`.

`stream`  

The stream to which to write.

The stream should be open and configured.

`opt`  

Options for writing the JSON data.

See JSONSerialization.WritingOptions for possible values.

`error`  

If an error occurs, upon return contains an `NSError` object with code NSPropertyListWriteInvalidError that describes the problem.

## Return Value

The number of bytes written to the stream, or `0` if an error occurs.

## See Also

### Creating JSON Data

class func data(withJSONObject: Any, options: JSONSerialization.WritingOptions) throws -> Data

Returns JSON data from a Foundation object.

struct WritingOptions

Options for writing JSON data.

class func isValidJSONObject(Any) -> Bool

Returns a Boolean value that indicates whether the serializer can convert a given object to JSON data.

