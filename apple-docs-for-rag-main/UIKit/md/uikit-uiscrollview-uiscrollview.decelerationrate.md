

- UIKit
- UIScrollView
-  UIScrollView.DecelerationRate 

Structure

# UIScrollView.DecelerationRate

Deceleration rates for the scroll view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct DecelerationRate
```

## Overview

You use these constants to set the value of the decelerationRate property.

## Topics

### Deceleration rates

static let normal: UIScrollView.DecelerationRate

The default deceleration rate for a scroll view.

static let fast: UIScrollView.DecelerationRate

A fast deceleration rate for a scroll view.

### Initializers

init(rawValue: CGFloat)

Creates a deceleration rate with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDragging: Bool

A Boolean value that indicates whether the user has begun scrolling the content.

var isDecelerating: Bool

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

var isScrollAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

