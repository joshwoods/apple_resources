

- SwiftUI
-  PagingScrollTargetBehavior 

Structure

# PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PagingScrollTargetBehavior
```

## Overview

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

## Topics

### Creating the target behavior

init()

Creates a paging scroll behavior.

## Relationships

### Conforms To

- ChartScrollTargetBehavior
- Copyable
- ScrollTargetBehavior

## See Also

### Defining scroll targets

func scrollTargetBehavior(some ScrollTargetBehavior) -> some View

Sets the scroll behavior of views scrollable in the provided axes.

func scrollTargetLayout(isEnabled: Bool) -> some View

Configures the outermost layout as a scroll target layout.

struct ScrollTarget

A type defining the target in which a scroll view should try and scroll to.

protocol ScrollTargetBehavior

A type that defines the scroll behavior of a scrollable view.

struct ScrollTargetBehaviorContext

The context in which a scroll target behavior updates its scroll target.

struct ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

struct AnyScrollTargetBehavior

A type-erased scroll target behavior.

