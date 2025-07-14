

- SwiftUI
-  AnyScrollTargetBehavior 

Structure

# AnyScrollTargetBehavior

A type-erased scroll target behavior.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct AnyScrollTargetBehavior
```

## Overview

Provide this to the scrollTargetBehavior(_:) modifier. When the underlying behavior changes, the scroll view to which this behavior applies will be updated.

Use this to dynamically control the scroll target behavior at runtime. For example, you could provide a paging behavior in compact size classes and a view aligned behavior otherwise.

```
@Environment(\.horizontalSizeClass) var sizeClass

var body: some View {
    ScrollView { ... }
        .scrollTargetBehavior(scrollTargetBehavior)
}

 var scrollTargetBehavior: some ScrollTargetBehavior {
    sizeClass == .compact
        ? AnyScrollTargetBehavior(.paging)
        : AnyScrollTargetBehavior(.viewAligned)
}
```

## Topics

### Initializers

init(some ScrollTargetBehavior)

Creates a new type-erase scroll target behavior.

### Instance Properties

var base: any ScrollTargetBehavior

The type-erased scroll target behavior.

## Relationships

### Conforms To

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

struct PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

struct ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

