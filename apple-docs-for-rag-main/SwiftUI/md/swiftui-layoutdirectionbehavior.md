

- SwiftUI
-  LayoutDirectionBehavior 

Enumeration

# LayoutDirectionBehavior

A description of what should happen when the layout direction changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum LayoutDirectionBehavior
```

## Overview

A `LayoutDirectionBehavior` can be used with the `layoutDirectionBehavior` view modifier or the `layoutDirectionBehavior` property of `Shape`.

## Topics

### Getting behaviors

case fixed

A behavior that doesn’t mirror when the layout direction changes.

static var mirrors: LayoutDirectionBehavior

A behavior that mirrors when the layout direction is right-to-left.

case mirrors(in: LayoutDirection)

A behavior that mirrors when the layout direction has the specified value.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Setting a layout direction

func layoutDirectionBehavior(LayoutDirectionBehavior) -> some View

Sets the behavior of this view for different layout directions.

var layoutDirection: LayoutDirection

The layout direction associated with the current environment.

enum LayoutDirection

A direction in which SwiftUI can lay out content.

