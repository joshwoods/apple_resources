

- BrowserEngineKit
-  BEScrollViewDelegate 

Protocol

# BEScrollViewDelegate

The protocol that browser scroll view delegates conform to.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
protocol BEScrollViewDelegate : UIScrollViewDelegate
```

## Topics

### Nesting sibling scroll views

func parentScrollView(for: BEScrollView) -> BEScrollView?

Indicates that a sibling scroll view in the view hierarchy acts as the scroll view’s container in the Document Object Model (DOM).

### Handling scroll events

func scrollView(BEScrollView, handle: BEScrollViewScrollUpdate, completion: (Bool) -> Void)

Handles a scroll update, optionally stopping the scroll view from reacting.

## Relationships

### Inherits From

- NSObjectProtocol
- UIScrollViewDelegate

## See Also

### Scroll view interaction

class BEScrollView

A scroll view that works with its delegate to handle nesting, and customize scroll interactions.

class BEScrollViewScrollUpdate

An object that represents a change in a scroll view’s scroll state.

