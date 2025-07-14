

- Foundation
- NSCoder
-  containsValue(forKey:) 

Instance Method

# containsValue(forKey:)

Returns a Boolean value that indicates whether an encoded value is available for a string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func containsValue(forKey key: String) -> Bool
```

## Discussion

Subclasses must override this method if they perform keyed coding.

The string is passed as `key`.

## See Also

### Inspecting a Coder

var allowsKeyedCoding: Bool

A Boolean value that indicates whether the receiver supports keyed coding of objects.

var decodingFailurePolicy: NSCoder.DecodingFailurePolicy

The action the coder should take when decoding fails.

enum DecodingFailurePolicy

Policies describing the action the coder should take when encountering decode failures.

