

- Foundation
- AttributedStringProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns a substring of the attributed string using a range to indicate the substring bounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(bounds: R) -> AttributedSubstring where R : RangeExpression, R.Bound == AttributedString.Index { get }
```

**Required**

