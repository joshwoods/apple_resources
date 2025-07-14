

- Core Animation
- CARenderer
-  beginFrame(atTime:timeStamp:) 

Instance Method

# beginFrame(atTime:timeStamp:)

Begin rendering a frame at the specified time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func beginFrame(
    atTime t: CFTimeInterval,
    timeStamp ts: UnsafeMutablePointer?
)
```

## Parameters 

`t`  

The layer time.

`ts`  

The display timestamp associated with timeInterval. Can be null.

## See Also

### Rendering a Frame

func updateBounds() -> CGRect

Returns the bounds of the update region that contains all pixels that will be rendered by the current frame.

func addUpdate(CGRect)

Adds the rectangle to the update region of the current frame.

func render()

Render the update region of the current frame to the target context.

func nextFrameTime() -> CFTimeInterval

Returns the time at which the next update should happen.

func endFrame()

Release any data associated with the current frame.

