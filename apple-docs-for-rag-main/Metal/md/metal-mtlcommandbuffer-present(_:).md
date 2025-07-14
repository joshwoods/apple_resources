

- Metal
- MTLCommandBuffer
-  present(\_:) 

Instance Method

# present(\_:)

Presents a drawable as early as possible.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func present(_ drawable: any MTLDrawable)
```

**Required** Default implementation provided.

## Parameters 

`drawable`  

An MTLDrawable instance that contains a texture the system can show on a display.

## Discussion

This convenience method calls the drawable’s present() method after the command queue schedules the command buffer for execution. The command buffer does this by adding a completion handler by calling its own addScheduledHandler(_:) method for you.

Important

You can only call this method before calling the command buffer’s commit() method.

## Default Implementations

### MTLCommandBuffer Implementations

func present(TextureResource.Drawable)

Presents a texture resource drawable as early as possible.

## See Also

### Presenting a Drawable

func present(any MTLDrawable, atTime: CFTimeInterval)

Presents a drawable at a specific time.

**Required**

func present(any MTLDrawable, afterMinimumDuration: CFTimeInterval)

Presents a drawable after the system presents the previous drawable for an amount of time.

**Required**

