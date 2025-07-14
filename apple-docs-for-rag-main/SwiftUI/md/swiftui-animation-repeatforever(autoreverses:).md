

- SwiftUI
- Animation
-  repeatForever(autoreverses:) 

Instance Method

# repeatForever(autoreverses:)

Repeats the animation for the lifespan of the view containing the animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func repeatForever(autoreverses: Bool = true) -> Animation
```

## Parameters 

`autoreverses`  

A Boolean value that indicates whether the animation sequence plays in reverse after playing forward.

## Return Value

An animation that continuously repeats.

## Discussion

Use this method to repeat the animation until the instance of the view no longer exists, or the view’s explicit or structural identity changes. For example, the following code continuously rotates a gear symbol for the lifespan of the view.

```
struct ContentView: View {
    @State private var rotationDegrees = 0.0

    private var animation: Animation {
        .linear
        .speed(0.1)
        .repeatForever(autoreverses: false)
    }

    var body: some View {
        Image(systemName: "gear")
            .font(.system(size: 86))
            .rotationEffect(.degrees(rotationDegrees))
            .onAppear {
                withAnimation(animation) {
                    rotationDegrees = 360.0
                }
            }
    }
}
```

 Video with custom controls. 

 Content description: A video that shows a gear that continuously rotates clockwise. 

Play 

## See Also

### Configuring an animation

func delay(TimeInterval) -> Animation

Delays the start of the animation by the specified number of seconds.

func repeatCount(Int, autoreverses: Bool) -> Animation

Repeats the animation for a specific number of times.

func speed(Double) -> Animation

Changes the duration of an animation by adjusting its speed.

