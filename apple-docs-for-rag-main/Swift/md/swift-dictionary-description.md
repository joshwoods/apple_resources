

- Swift
- Dictionary
-  description 

Instance Property

# description

A string that represents the contents of the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var description: String { get }
```

Available when `Key` conforms to `Hashable`.

## See Also

### Describing a Dictionary

var debugDescription: String

A string that represents the contents of the dictionary, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the dictionary.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

