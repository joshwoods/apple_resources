

- Swift
- Float
-  debugDescription 

Instance Property

# debugDescription

A textual representation of the value, suitable for debugging.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var debugDescription: String { get }
```

## Discussion

This property has the same value as the `description` property, except that NaN values are printed in an extended format.

## See Also

### Describing a Float

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var description: String

A textual representation of the value.

var customMirror: Mirror

A mirror that reflects the `Float` instance.

var hashValue: Int

The hash value.

