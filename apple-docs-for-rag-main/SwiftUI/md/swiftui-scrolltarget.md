

- SwiftUI
-  ScrollTarget 

Structure

# ScrollTarget

A type defining the target in which a scroll view should try and scroll to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ScrollTarget
```

## Topics

### Getting the scroll target

var anchor: UnitPoint?

The anchor to which the rect should be aligned within the visible region of the scrollable view.

var rect: CGRect

The rect that a scrollable view should try and have contained.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Defining scroll targets

func scrollTargetBehavior(some ScrollTargetBehavior) -> some View

Sets the scroll behavior of views scrollable in the provided axes.

func scrollTargetLayout(isEnabled: Bool) -> some View

Configures the outermost layout as a scroll target layout.

protocol ScrollTargetBehavior

A type that defines the scroll behavior of a scrollable view.

struct ScrollTargetBehaviorContext

The context in which a scroll target behavior updates its scroll target.

struct PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

struct ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

struct AnyScrollTargetBehavior

A type-erased scroll target behavior.

