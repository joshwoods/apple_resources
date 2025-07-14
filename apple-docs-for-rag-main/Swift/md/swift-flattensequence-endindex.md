

- Swift
- FlattenSequence
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: FlattenSequence.Index { get }
```

Available when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

## Discussion

`endIndex` is not a valid argument to `subscript`, and is always reachable from `startIndex` by zero or more applications of `index(after:)`.

