

- SpriteKit
-  SKViewDelegate 

Protocol

# SKViewDelegate

Methods to take custom control over the view’s render rate.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
protocol SKViewDelegate : NSObjectProtocol
```

## Mentioned in 

Getting Started with Nodes

## Overview

By setting a SpriteKit view’s `delegate` with an object that implements SKViewDelegate, you can precisely control the frame rate of a game or app. You may choose to do this to maintain a consistent frame rate for computationally intensive code or for special effects such as simulating cine film.

The following Swift code shows an example of a class that implements the SpriteKit view delegate protocol to reduce the frame rate to a specified value. With each call of view(_:shouldRenderAtTime:), it checks the time since the last render and if that value exceeds the required frame duration (`1 / fps`), the method returns true and the frame is rendered.

```
class ViewDelegate: NSObject, SKViewDelegate {
    var lastRenderTime: TimeInterval = 0

    let fps: TimeInterval = 3

    public func view(_ view: SKView, shouldRenderAtTime time: TimeInterval) -> Bool {

        if time - lastRenderTime >= 1 / fps {
            lastRenderTime = time
            return true
        }
        else {
            return false
        }

    }
}
```

The return value of view(_:shouldRenderAtTime:) doesn’t change the speed of physics simulations and actions in a SpriteKit scene. However, if you return false, SpriteKit will skip updates and SKSceneDelegate methods are not called.

## Topics

### Instance Methods

func view(SKView, shouldRenderAtTime: TimeInterval) -> Bool

Specifies whether the view should render at the given time.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Controlling the Timing of a Scene’s Rendering

var isPaused: Bool

A Boolean value that indicates whether the view’s scene animations are paused.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var delegate: (any SKViewDelegate)?

A delegate that allows dynamic control of the view’s render rate.

var frameInterval: Int

The number of frames that must pass before the scene is called to update its contents.

Deprecated

var preferredFrameRate: FloatDeprecated

