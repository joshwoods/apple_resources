

- SwiftUI
-  LayoutSubviews 

Structure

# LayoutSubviews

A collection of proxy values that represent the subviews of a layout view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LayoutSubviews
```

## Overview

You receive a `LayoutSubviews` input to your implementations of Layout protocol methods, like placeSubviews(in:proposal:subviews:cache:) and sizeThatFits(proposal:subviews:cache:). The `subviews` parameter (which the protocol aliases to the Layout.Subviews type) is a collection that contains proxies for the layout’s subviews (of type LayoutSubview). The proxies appear in the collection in the same order that they appear in the ViewBuilder input to the layout container. Use the proxies to perform layout operations.

Access the proxies in the collection as you would the contents of any Swift random-access collection. For example, you can enumerate all of the subviews and their indices to inspect or operate on them:

```
for (index, subview) in subviews.enumerated() {
    // ...
}
```

## Topics

### Getting the layout direction

var layoutDirection: LayoutDirection

The layout direction inherited by the container view.

### Accessing subviews

subscript(_:)

Gets the subview proxies in the specified range.

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

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Creating a custom layout container

Composing custom layouts with SwiftUI

Arrange views in your app’s interface using layout tools that SwiftUI provides.

protocol Layout

A type that defines the geometry of a collection of views.

struct LayoutSubview

A proxy that represents one subview of a layout.

