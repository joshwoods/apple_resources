

- Swift
- Dictionary
-  customMirror 

Instance Property

# customMirror

A mirror that reflects the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var customMirror: Mirror { get }
```

Available when `Key` conforms to `Hashable`.

## See Also

### Describing a Dictionary

var description: String

A string that represents the contents of the dictionary.

var debugDescription: String

A string that represents the contents of the dictionary, suitable for debugging.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

