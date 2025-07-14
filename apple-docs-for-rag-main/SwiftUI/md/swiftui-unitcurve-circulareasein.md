

- SwiftUI
- UnitCurve
-  circularEaseIn 

Type Property

# circularEaseIn

A curve that starts out slowly, then speeds up as it finishes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let circularEaseIn: UnitCurve
```

## Discussion

The shape of the curve is equal to the fourth (bottom right) quadrant of a unit circle.

## See Also

### Getting easing curves

static let easeIn: UnitCurve

A bezier curve that starts out slowly, then speeds up as it finishes.

static let easeOut: UnitCurve

A bezier curve that starts out quickly, then slows down as it approaches the end.

static let easeInOut: UnitCurve

A bezier curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

static let circularEaseOut: UnitCurve

A circular curve that starts out quickly, then slows down as it approaches the end.

static let circularEaseInOut: UnitCurve

A circular curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

