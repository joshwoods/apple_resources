

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.UTF8View
-  endIndex 

Instance Property

# endIndex

The “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var endIndex: Int { get }
```

## Discussion

If the collection is empty, `endIndex` is equal to `startIndex`.

