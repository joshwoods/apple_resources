

- Swift
- Substring
-  isContiguousUTF8 

Instance Property

# isContiguousUTF8

Returns whether this string is capable of providing access to validly-encoded UTF-8 contents in contiguous memory in O(1) time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isContiguousUTF8: Bool { get }
```

## Discussion

Contiguous strings always operate in O(1) time for withUTF8 and always give a result for String.UTF8View.withContiguousStorageIfAvailable. Contiguous strings also benefit from fast-paths and better optimizations.

