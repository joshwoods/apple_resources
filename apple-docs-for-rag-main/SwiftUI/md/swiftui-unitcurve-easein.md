

- SwiftUI
- UnitCurve
-  easeIn 

Type Property

# easeIn

A bezier curve that starts out slowly, then speeds up as it finishes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let easeIn: UnitCurve
```

## Discussion

The start and end control points are located at (x: 0.42, y: 0) and (x: 1, y: 1).

## See Also

### Getting easing curves

static let easeOut: UnitCurve

A bezier curve that starts out quickly, then slows down as it approaches the end.

static let easeInOut: UnitCurve

A bezier curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

static let circularEaseIn: UnitCurve

A curve that starts out slowly, then speeds up as it finishes.

static let circularEaseOut: UnitCurve

A circular curve that starts out quickly, then slows down as it approaches the end.

static let circularEaseInOut: UnitCurve

A circular curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

