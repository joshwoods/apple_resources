

- SwiftUI
- LayoutSubviews
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Gets the subview proxies in the specified range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
subscript(bounds: Range) -> LayoutSubviews { get }
```

Show all declarations

## See Also

### Accessing subviews

var startIndex: Int

The index of the first subview.

var endIndex: Int

An index that’s one higher than the last subview.

typealias Element

A type that contains a proxy value.

typealias Index

A type that you can use to index proxy values.

typealias SubSequence

A type that contains a subsequence of proxy values.

