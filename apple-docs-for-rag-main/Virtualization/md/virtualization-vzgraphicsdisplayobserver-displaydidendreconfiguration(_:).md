

- Virtualization
- VZGraphicsDisplayObserver
-  displayDidEndReconfiguration(\_:) 

Instance Method

# displayDidEndReconfiguration(\_:)

The method the framework calls when the reconfiguration operation ends.

macOS 14.0+

``` source
optional func displayDidEndReconfiguration(_ display: VZGraphicsDisplay)
```

## Parameters 

`display`  

The VZGraphicsDisplay whose state is changing.

## Discussion

Frame updates have arrived at the most recently requested display size and configuration.

The framework invokes this method on the VM’s queue.

## See Also

### Reacting to changes in display configuration

func displayDidBeginReconfiguration(VZGraphicsDisplay)

The method the framework calls when the reconfiguration operation has begun.

