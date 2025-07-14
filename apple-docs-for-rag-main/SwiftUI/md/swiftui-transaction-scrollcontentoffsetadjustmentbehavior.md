

- SwiftUI
- Transaction
-  scrollContentOffsetAdjustmentBehavior 

Instance Property

# scrollContentOffsetAdjustmentBehavior

The behavior a scroll view will have regarding content offset adjustments for the current transaction.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var scrollContentOffsetAdjustmentBehavior: ScrollContentOffsetAdjustmentBehavior { get set }
```

## Discussion

A scroll view may automatically adjust its content offset based on the current context. The absolute offset may be adjusted to keep content in relatively the same place. For example, when scrolled to the bottom, a scroll view may keep the bottom edge scrolled to the bottom when the overall size of its content changes.

Use this property to disable these kinds of adjustments when needed.

