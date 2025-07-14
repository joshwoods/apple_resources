

- Swift
- UnsafeRawBufferPointer
-  endIndex 

Instance Property

# endIndex

The “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: UnsafeRawBufferPointer.Index { get }
```

## Discussion

The `endIndex` property of an `UnsafeRawBufferPointer` instance is always identical to `count`.

