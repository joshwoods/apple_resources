

- SwiftUI
-  ScrollBounceBehavior 

Structure

# ScrollBounceBehavior

The ways that a scrollable view can bounce when it reaches the end of its content.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct ScrollBounceBehavior
```

## Overview

Use the scrollBounceBehavior(_:axes:) view modifier to set a value of this type for a scrollable view, like a ScrollView or a List. The value configures the bounce behavior when people scroll to the end of the view’s content.

You can configure each scrollable axis to use a different bounce mode.

## Topics

### Bounce behaviors

static var automatic: ScrollBounceBehavior

The automatic behavior.

static var always: ScrollBounceBehavior

The scrollable view always bounces.

static var basedOnSize: ScrollBounceBehavior

The scrollable view bounces when its content is large enough to require scrolling.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring scroll bounce behavior

func scrollBounceBehavior(ScrollBounceBehavior, axes: Axis.Set) -> some View

Configures the bounce behavior of scrollable views along the specified axis.

var horizontalScrollBounceBehavior: ScrollBounceBehavior

The scroll bounce mode for the horizontal axis of scrollable views.

var verticalScrollBounceBehavior: ScrollBounceBehavior

The scroll bounce mode for the vertical axis of scrollable views.

