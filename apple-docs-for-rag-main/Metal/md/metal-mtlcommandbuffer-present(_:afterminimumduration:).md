

- Metal
- MTLCommandBuffer
-  present(\_:afterMinimumDuration:) 

Instance Method

# present(\_:afterMinimumDuration:)

Presents a drawable after the system presents the previous drawable for an amount of time.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.4+macOS 10.15.4+tvOS 10.2+visionOS 1.0+

``` source
func present(
    _ drawable: any MTLDrawable,
    afterMinimumDuration duration: CFTimeInterval
)
```

**Required**

## Parameters 

`drawable`  

An MTLDrawable instance that contains a texture the system can show on a display.

`duration`  

The shortest display time you want the system to give to the previous drawable before presenting this one.

## Discussion

This convenience method calls the drawable’s present(afterMinimumDuration:) method after the command queue schedules the command buffer for execution. The command buffer does this by adding a completion handler by calling its own addScheduledHandler(_:) method for you.

Important

You can only call this method before calling the command buffer’s commit() method.

## See Also

### Presenting a Drawable

func present(any MTLDrawable)

Presents a drawable as early as possible.

**Required** Default implementation provided.

func present(any MTLDrawable, atTime: CFTimeInterval)

Presents a drawable at a specific time.

**Required**

