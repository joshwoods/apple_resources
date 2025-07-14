

- SwiftUI
- ScrollTargetBehavior
-  paging 

Type Property

# paging

The scroll behavior that aligns scroll targets to container-based geometry.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var paging: PagingScrollTargetBehavior { get }
```

Available when `Self` is `PagingScrollTargetBehavior`.

## Discussion

In the following example, every view in the lazy stack is flexible in both directions and the scroll view settles to container-aligned boundaries.

```
ScrollView {
    LazyVStack(spacing: 0.0) {
        ForEach(items) { item in
            FullScreenItem(item)
        }
    }
}
.scrollTargetBehavior(.paging)
```

## See Also

### Getting the scroll target behavior

static var viewAligned: ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

static func viewAligned(limitBehavior: ViewAlignedScrollTargetBehavior.LimitBehavior) -> Self

The scroll behavior that aligns scroll targets to view-based geometry.

