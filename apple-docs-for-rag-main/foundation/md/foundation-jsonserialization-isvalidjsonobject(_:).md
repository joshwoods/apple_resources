

- Foundation
- JSONSerialization
-  isValidJSONObject(\_:) 

Type Method

# isValidJSONObject(\_:)

Returns a Boolean value that indicates whether the serializer can convert a given object to JSON data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func isValidJSONObject(_ obj: Any) -> Bool
```

## Parameters 

`obj`  

The object to test.

## Return Value

`true` if `obj` can be converted to JSON data; otherwise, `false`.

## See Also

### Creating JSON Data

class func data(withJSONObject: Any, options: JSONSerialization.WritingOptions) throws -> Data

Returns JSON data from a Foundation object.

class func writeJSONObject(Any, to: OutputStream, options: JSONSerialization.WritingOptions, error: NSErrorPointer) -> Int

Writes a given JSON object to a stream.

struct WritingOptions

Options for writing JSON data.

