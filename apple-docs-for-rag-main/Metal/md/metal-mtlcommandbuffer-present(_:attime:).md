

- Metal
- MTLCommandBuffer
-  present(\_:atTime:) 

Instance Method

# present(\_:atTime:)

Presents a drawable at a specific time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func present(
    _ drawable: any MTLDrawable,
    atTime presentationTime: CFTimeInterval
)
```

**Required**

## Parameters 

`drawable`  

An MTLDrawable instance that contains a texture the system can show on a display.

`presentationTime`  

The Mach absolute time, in seconds, that you want to present the drawable.

## Discussion

This convenience method calls the drawable’s present(at:) method after the command queue schedules the command buffer for execution. The command buffer does this by adding a completion handler by calling its own addScheduledHandler(_:) method for you.

Important

You can only call this method before calling the command buffer’s commit() method.

## See Also

### Presenting a Drawable

func present(any MTLDrawable)

Presents a drawable as early as possible.

**Required** Default implementation provided.

func present(any MTLDrawable, afterMinimumDuration: CFTimeInterval)

Presents a drawable after the system presents the previous drawable for an amount of time.

**Required**

