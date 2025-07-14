

- Swift
- Repeated
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: Repeated.Index { get }
```

## Discussion

In a `Repeated` collection, `endIndex` is always equal to `count`. If the collection is empty, `endIndex` is equal to `startIndex`.

