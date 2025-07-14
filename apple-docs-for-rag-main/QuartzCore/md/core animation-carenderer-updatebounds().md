

- Core Animation
- CARenderer
-  updateBounds() 

Instance Method

# updateBounds()

Returns the bounds of the update region that contains all pixels that will be rendered by the current frame.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func updateBounds() -> CGRect
```

## Return Value

The bounds of the update region..

## Discussion

Initially `updateBounds` will include all differences between the current frame and the previously rendered frame.

## See Also

### Rendering a Frame

func beginFrame(atTime: CFTimeInterval, timeStamp: UnsafeMutablePointer&lt;CVTimeStamp>?)

Begin rendering a frame at the specified time.

func addUpdate(CGRect)

Adds the rectangle to the update region of the current frame.

func render()

Render the update region of the current frame to the target context.

func nextFrameTime() -> CFTimeInterval

Returns the time at which the next update should happen.

func endFrame()

Release any data associated with the current frame.

