

- Swift
- String
- String.UTF8View
-  endIndex 

Instance Property

# endIndex

The “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: String.UTF8View.Index { get }
```

## Discussion

In an empty UTF-8 view, `endIndex` is equal to `startIndex`.

