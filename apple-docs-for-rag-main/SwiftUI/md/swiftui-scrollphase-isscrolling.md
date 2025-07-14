

- SwiftUI
- ScrollPhase
-  isScrolling 

Instance Property

# isScrolling

Whether the scroll view is actively scrolling.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var isScrolling: Bool { get }
```

## Discussion

This convenience is equivalent to `phase != .idle`.

