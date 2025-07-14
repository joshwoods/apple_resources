

- Swift
-  repeatElement(\_:count:) 

Function

# repeatElement(\_:count:)

Creates a collection containing the specified number of the given element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func repeatElement(
    _ element: T,
    count n: Int
) -> Repeated
```

## Parameters 

`element`  

The element to repeat.

## Return Value

A collection that contains `count` elements that are all `element`.

## Discussion

The following example creates a `Repeated` collection containing five zeroes:

```
let zeroes = repeatElement(0, count: 5)
for x in zeroes {
    print(x)
}
// 0
// 0
// 0
// 0
// 0
```

## See Also

### Special-Use Collections

struct CollectionOfOne

A collection containing a single element.

struct EmptyCollection

A collection whose element type is `Element` but that is always empty.

struct KeyValuePairs

A lightweight collection of key-value pairs.

typealias DictionaryLiteral

