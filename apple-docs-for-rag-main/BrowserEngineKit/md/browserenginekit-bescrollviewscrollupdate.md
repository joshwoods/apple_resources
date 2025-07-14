

- BrowserEngineKit
-  BEScrollViewScrollUpdate 

Class

# BEScrollViewScrollUpdate

An object that represents a change in a scroll view’s scroll state.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
class BEScrollViewScrollUpdate
```

## Overview

When a person scrolls a BEScrollView, the view’s delegate receives the scrollView(_:handle:completion:) method. The `handle` parameter is an instance of `BEScrollViewScrollUpdate` that describes the scroll activity.

Your app can continue to receive `BEScrollViewScrollUpdate` objects after the person completes their scroll gesture, as the scrolling decelerates.

Important

`BEScrollViewScrollUpdate` isn’t thread-safe, and the system uses the same object for multiple scroll updates. When you receive a scroll update, immediately get the information you need on the main queue before any other processing.

## Topics

### Retrieving scroll state information

var timestamp: TimeInterval

The time at which the scroll update occurred.

var phase: BEScrollViewScrollUpdate.Phase

The point in the scrolling lifecycle represented by the scroll update.

enum Phase

The phase of a scroll update in a scroll gesture’s lifecycle.

### Transforming coordinates

func location(in: UIView?) -> CGPoint

Returns the coordinates of the scroll update in the given view’s bounds.

func translation(in: UIView?) -> CGPoint

Returns the amount of scrolling in the scroll update in the given view’s coordinates.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Scroll view interaction

class BEScrollView

A scroll view that works with its delegate to handle nesting, and customize scroll interactions.

protocol BEScrollViewDelegate

The protocol that browser scroll view delegates conform to.

