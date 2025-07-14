

- SwiftUI
-  ScrollTargetBehaviorContext 

Structure

# ScrollTargetBehaviorContext

The context in which a scroll target behavior updates its scroll target.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@dynamicMemberLookup
struct ScrollTargetBehaviorContext
```

## Topics

### Getting the scroll target behavior context

var axes: Axis.Set

The axes in which the scrollable view is scrollable.

var containerSize: CGSize

The size of the container of the scrollable view.

var contentSize: CGSize

The size of the content of the scrollable view.

var originalTarget: ScrollTarget

The original target when the scroll gesture began.

var velocity: CGVector

The current velocity of the scrollable view’s scroll gesture.

### Accessing the context

subscript&lt;T>(dynamicMember _: KeyPath&lt;EnvironmentValues, T>) -> T

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

struct PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

struct ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

struct AnyScrollTargetBehavior

A type-erased scroll target behavior.

