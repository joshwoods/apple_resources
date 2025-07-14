

- Virtualization
- VZGraphicsDisplayObserver
-  displayDidBeginReconfiguration(\_:) 

Instance Method

# displayDidBeginReconfiguration(\_:)

The method the framework calls when the reconfiguration operation has begun.

macOS 14.0+

``` source
optional func displayDidBeginReconfiguration(_ display: VZGraphicsDisplay)
```

## Parameters 

`display`  

The VZGraphicsDisplay whose state is changing.

## Discussion

The framework issued a configuration change, such as a resize, and you can expect new frames with a new size or configuration.

The framework invokes this method on the VM’s queue.

## See Also

### Reacting to changes in display configuration

func displayDidEndReconfiguration(VZGraphicsDisplay)

The method the framework calls when the reconfiguration operation ends.

