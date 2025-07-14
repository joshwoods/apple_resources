

- WatchKit
-  WKSwipeGestureRecognizerDirection 

Structure

# WKSwipeGestureRecognizerDirection

Constants indicating the direction of a swipe.

watchOS 3.0+

``` source
struct WKSwipeGestureRecognizerDirection
```

## Topics

### Constants

static var right: WKSwipeGestureRecognizerDirection

The touch moves from left to right. This direction is the default.

static var left: WKSwipeGestureRecognizerDirection

The touch moves from right to left.

static var up: WKSwipeGestureRecognizerDirection

The touch moves upward.

static var down: WKSwipeGestureRecognizerDirection

The touch moves downward.

### Initializers

init(rawValue: UInt)

Returns a new direction constant based on the provided raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

