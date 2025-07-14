

- Foundation
- JSONSerialization
-  data(withJSONObject:options:) 

Type Method

# data(withJSONObject:options:)

Returns JSON data from a Foundation object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func data(
    withJSONObject obj: Any,
    options opt: JSONSerialization.WritingOptions = []
) throws -> Data
```

## Parameters 

`obj`  

The object from which to generate JSON data. Must not be `nil`.

`opt`  

Options for creating the JSON data.

See JSONSerialization.WritingOptions for possible values.

## Return Value

JSON data for `obj`, or `nil` if an internal error occurs. The resulting data is encoded in UTF-8.

## Discussion

If `obj` can’t produce valid JSON, JSONSerialization throws an exception. This exception occurs prior to parsing and represents a programming error, not an internal error. Before calling this method, you should check whether the input can produce valid JSON by using isValidJSONObject(_:).

Setting the prettyPrinted option generates JSON with white space designed to make the output more readable. If this option isn’t set, JSONSerialization generates the most compact possible JSON.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating JSON Data

class func writeJSONObject(Any, to: OutputStream, options: JSONSerialization.WritingOptions, error: NSErrorPointer) -> Int

Writes a given JSON object to a stream.

struct WritingOptions

Options for writing JSON data.

class func isValidJSONObject(Any) -> Bool

Returns a Boolean value that indicates whether the serializer can convert a given object to JSON data.

