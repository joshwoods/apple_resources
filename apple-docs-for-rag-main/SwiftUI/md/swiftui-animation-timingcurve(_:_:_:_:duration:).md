

- SwiftUI
- Animation
-  timingCurve(\_:\_:\_:\_:duration:) 

Type Method

# timingCurve(\_:\_:\_:\_:duration:)

An animation created from a cubic Bézier timing curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func timingCurve(
    _ p1x: Double,
    _ p1y: Double,
    _ p2x: Double,
    _ p2y: Double,
    duration: TimeInterval = 0.35
) -> Animation
```

## Parameters 

`p1x`  

The x-coordinate of the first control point of the cubic Bézier curve.

`p1y`  

The y-coordinate of the first control point of the cubic Bézier curve.

`p2x`  

The x-coordinate of the second control point of the cubic Bézier curve.

`p2y`  

The y-coordinate of the second control point of the cubic Bézier curve.

`duration`  

The length of time, expressed in seconds, the animation takes to complete.

## Return Value

A cubic Bézier timing curve animation.

## Discussion

Use this method to create a timing curve based on the control points of a cubic Bézier curve. A cubic Bézier timing curve consists of a line whose starting point is `(0, 0)` and whose end point is `(1, 1)`. Two additional control points, `(p1x, p1y)` and `(p2x, p2y)`, define the shape of the curve.

The slope of the line defines the speed of the animation at that point in time. A steep slopes causes the animation to appear to run faster, while a shallower slope appears to run slower. The following illustration shows a timing curve where the animation starts and finishes fast, but appears slower through the middle section of the animation.

The following code uses the timing curve from the previous illustration to animate a Circle as its size changes.

```
struct ContentView: View {
    @State private var scale = 1.0

    var body: some View {
        VStack {
            Circle()
                .scaleEffect(scale)
                .animation(
                    .timingCurve(0.1, 0.75, 0.85, 0.35, duration: 2.0),
                    value: scale)

            Button("Animate") {
                if scale == 1.0 {
                    scale = 0.25
                } else {
                    scale = 1.0
                }
            }
        }
    }
}
```

 Video with custom controls. 

 Content description: A video that shows a circle shrinking then growing to its original size using a timing curve animation. The first control point of the time curve is (0.1, 0.75) and the second is (0.85, 0.35). 

Play 

## See Also

### Creating custom animations

init&lt;A>(A)

Create an `Animation` that contains the specified custom animation.

static func timingCurve(UnitCurve, duration: TimeInterval) -> Animation

Creates a new animation with speed controlled by the given curve.

