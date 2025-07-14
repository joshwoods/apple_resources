

- AppKit
- NSTextInputContext
-  deactivate() 

Instance Method

# deactivate()

Deactivates the receiver.

macOS 10.6+

``` source
func deactivate()
```

## Discussion

You should not call this method directly; it is invoked by the system. It is provided as an override point for subclasses.

## See Also

### Activating the Input Context

func activate()

Activates the receiver.

