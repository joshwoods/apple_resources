

- Swift
- ContiguousArray
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startIndex: Int { get }
```

## Discussion

For an instance of `ContiguousArray`, `startIndex` is always zero. If the array is empty, `startIndex` is equal to `endIndex`.

