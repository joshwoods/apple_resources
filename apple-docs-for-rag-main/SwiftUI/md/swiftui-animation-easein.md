

- SwiftUI
- Animation
-  easeIn 

Type Property

# easeIn

An animation that starts slowly and then increases speed towards the end of the movement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var easeIn: Animation { get }
```

## Return Value

An ease-in animation with the default duration.

## Discussion

An easing animation provides motion with a natural feel by varying the acceleration and deceleration of the animation, which matches how things tend to move in reality. With an ease in animation, the motion starts slowly and increases its speed towards the end.

The `easeIn` animation has a default duration of 0.35 seconds. To specify a different duration, use easeIn(duration:).

The following code shows an example of animating the size changes of a Circle using the ease in animation.

```
struct ContentView: View {
    @State private var scale = 0.5

    var body: some View {
        VStack {
            Circle()
                .scale(scale)
                .animation(.easeIn, value: scale)
            HStack {
                Button("+") { scale += 0.1 }
                Button("-") { scale -= 0.1 }
            }
        }
    }
}
```

 Video with custom controls. 

 Content description: A video that shows a circle enlarging, then shrinking to its original size using an ease-in animation. 

Play 

## See Also

### Getting eased animations

static func easeIn(duration: TimeInterval) -> Animation

An animation with a specified duration that starts slowly and then increases speed towards the end of the movement.

static var easeOut: Animation

An animation that starts quickly and then slows towards the end of the movement.

static func easeOut(duration: TimeInterval) -> Animation

An animation with a specified duration that starts quickly and then slows towards the end of the movement.

static var easeInOut: Animation

An animation that combines the behaviors of in and out easing animations.

static func easeInOut(duration: TimeInterval) -> Animation

An animation with a specified duration that combines the behaviors of in and out easing animations.

