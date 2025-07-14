

- Swift
- Set
-  customMirror 

Instance Property

# customMirror

A mirror that reflects the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var customMirror: Mirror { get }
```

Available when `Element` conforms to `Hashable`.

## See Also

### Describing a Set

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var description: String

A string that represents the contents of the set.

var debugDescription: String

A string that represents the contents of the set, suitable for debugging.

