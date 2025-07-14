

- Swift
- Array
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## See Also

### Describing an Array

var description: String

A textual representation of the array and its elements.

var debugDescription: String

A textual representation of the array and its elements, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the array.

