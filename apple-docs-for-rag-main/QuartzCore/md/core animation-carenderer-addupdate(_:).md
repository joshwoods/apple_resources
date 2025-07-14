

- Core Animation
- CARenderer
-  addUpdate(\_:) 

Instance Method

# addUpdate(\_:)

Adds the rectangle to the update region of the current frame.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func addUpdate(_ r: CGRect)
```

## Parameters 

`r`  

A rectangle defining the region to be added to the update region.

## See Also

### Rendering a Frame

func beginFrame(atTime: CFTimeInterval, timeStamp: UnsafeMutablePointer&lt;CVTimeStamp>?)

Begin rendering a frame at the specified time.

func updateBounds() -> CGRect

Returns the bounds of the update region that contains all pixels that will be rendered by the current frame.

func render()

Render the update region of the current frame to the target context.

func nextFrameTime() -> CFTimeInterval

Returns the time at which the next update should happen.

func endFrame()

Release any data associated with the current frame.

