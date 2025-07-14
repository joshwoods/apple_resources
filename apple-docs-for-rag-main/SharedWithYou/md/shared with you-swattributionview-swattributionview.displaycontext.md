

- Shared With You
- SWAttributionView
-  SWAttributionView.DisplayContext 

Enumeration

# SWAttributionView.DisplayContext

The context for the content that influences the ranking of this view’s highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum DisplayContext
```

## Mentioned in 

Making your app content shareable

## Overview

Set the appropriate display context on SWAttributionView before the system adds the view to a window. This informs the system about how the user is consuming the attributed content, and influences future relevancy ranking of the SWHighlight for this view.

## Topics

### Context styles

case summary

Indicates that the system is offering the attributed content shown along with this view to the user for consumption.

case detail

Indicates that the attributed content shown along with this view is being actively consumed by the user.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the view

enum BackgroundStyle

The background styling of the attribution view’s contents.

enum HorizontalAlignment

The horizontal alignment of attribution view’s contents.

