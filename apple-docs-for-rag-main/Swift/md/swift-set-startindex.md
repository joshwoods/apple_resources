

- Swift
- Set
-  startIndex 

Instance Property

# startIndex

The starting position for iterating members of the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startIndex: Set.Index { get }
```

Available when `Element` conforms to `Hashable`.

## Discussion

If the set is empty, `startIndex` is equal to `endIndex`.

