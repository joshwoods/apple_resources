

- Metal
- MTLDrawable
-  present() 

Instance Method

# present()

Presents the drawable onscreen as soon as possible.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func present()
```

**Required**

## Discussion

When a command queue schedules a command buffer for execution, it tracks whether any commands in that command buffer need to render or write to the drawable object. When you call this method, the drawable presents its contents as soon as possible after all scheduled render or write requests for that drawable are complete.

Note

To avoid presenting a drawable before any work is scheduled, or to avoid holding on to a drawable longer than necessary, call a command buffer’s present(_:) method instead of this method. The present(_:) method is a convenience method that calls the drawable’s present() method after the command queue schedules that command buffer for execution.

## See Also

### Presenting the Drawable

func present(afterMinimumDuration: CFTimeInterval)

Presents the drawable onscreen as soon as possible after a previous drawable is visible for the specified duration.

**Required**

func present(at: CFTimeInterval)

Presents the drawable onscreen at a specific host time.

**Required**

