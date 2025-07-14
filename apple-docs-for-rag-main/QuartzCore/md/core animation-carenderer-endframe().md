

- Core Animation
- CARenderer
-  endFrame() 

Instance Method

# endFrame()

Release any data associated with the current frame.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func endFrame()
```

## See Also

### Rendering a Frame

func beginFrame(atTime: CFTimeInterval, timeStamp: UnsafeMutablePointer&lt;CVTimeStamp>?)

Begin rendering a frame at the specified time.

func updateBounds() -> CGRect

Returns the bounds of the update region that contains all pixels that will be rendered by the current frame.

func addUpdate(CGRect)

Adds the rectangle to the update region of the current frame.

func render()

Render the update region of the current frame to the target context.

func nextFrameTime() -> CFTimeInterval

Returns the time at which the next update should happen.

