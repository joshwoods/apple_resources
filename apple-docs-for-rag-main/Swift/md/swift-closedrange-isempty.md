

- Swift
- ClosedRange
-  isEmpty 

Instance Property

# isEmpty

A Boolean value indicating whether the range contains no elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isEmpty: Bool { get }
```

Available when `Bound` conforms to `Comparable`.

## Discussion

Because a closed range cannot represent an empty range, this property is always `false`.

## See Also

### Inspecting a Range

let lowerBound: Bound

The range’s lower bound.

let upperBound: Bound

The range’s upper bound.

