

- Swift
- Dictionary
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startIndex: Dictionary.Index { get }
```

Available when `Key` conforms to `Hashable`.

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

Complexity

Amortized O(1) if the dictionary does not wrap a bridged `NSDictionary`. If the dictionary wraps a bridged `NSDictionary`, the performance is unspecified.

