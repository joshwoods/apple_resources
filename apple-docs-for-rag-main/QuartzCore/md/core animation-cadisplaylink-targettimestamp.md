

- Core Animation
- CADisplayLink
-  targetTimestamp 

Instance Property

# targetTimestamp

The time interval that represents when the next frame displays.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 14.0+tvOS 10.0+visionOS 1.0+

``` source
var targetTimestamp: CFTimeInterval { get }
```

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## Discussion

You can use the target timestamp to cancel or pause long running processes that may overrun the available time between frames in order to maintain a consistent frame rate.

The following code shows how you can create a display link and register it with a run loop. The ``` step(``displayLink:) ``` function attempts to sum the square roots of all numbers up to max, but with each iteration checks the current time (CACurrentMediaTime()) against the targetTimestamp. If the time taken to complete the calculation is later than the target timestamp, the function breaks the loop:

```
func createDisplayLink() {
    let displayLink = CADisplayLink(target: self,
                                    selector: #selector(step))
    displayLink.add(to: .main,
                    forMode: .defaultRunLoopMode)
}

func step(displayLink: CADisplayLink) {
    var sqrtSum = 0.0
    for i in 0 ..= displayLink.targetTimestamp) {
            print("break at i =", i)
            break
        }
    }
}
```

## See Also

### Configuring a Display Link

var duration: CFTimeInterval

The time interval between screen refresh updates.

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFramesPerSecond: Int

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

Deprecated

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

