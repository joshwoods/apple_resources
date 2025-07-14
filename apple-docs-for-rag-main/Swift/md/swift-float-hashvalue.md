

- Swift
- Float
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Describing a Float

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var description: String

A textual representation of the value.

var debugDescription: String

A textual representation of the value, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Float` instance.

