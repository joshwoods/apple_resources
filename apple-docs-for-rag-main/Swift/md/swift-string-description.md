

- Swift
- String
-  description 

Instance Property

# description

The value of this string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var description: String { get }
```

## Discussion

Using this property directly is discouraged. Instead, use simple assignment to create a new constant or variable equal to this string.

## See Also

### Describing a String

var debugDescription: String

A representation of the string that is suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `String` instance.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

