

- Swift
- Set
-  endIndex 

Instance Property

# endIndex

The “past the end” position for the set—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: Set.Index { get }
```

Available when `Element` conforms to `Hashable`.

## Discussion

If the set is empty, `endIndex` is equal to `startIndex`.

