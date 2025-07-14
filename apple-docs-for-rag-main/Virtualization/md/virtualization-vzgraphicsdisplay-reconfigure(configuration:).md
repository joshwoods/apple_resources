

- Virtualization
- VZGraphicsDisplay
-  reconfigure(configuration:) 

Instance Method

# reconfigure(configuration:)

Reconfigure this display with the new display configuration you provide.

macOS 14.0+

``` source
func reconfigure(configuration: VZGraphicsDisplayConfiguration) throws
```

## Parameters 

`configuration`  

The new VZGraphicsDisplayConfiguration configuration.

## Discussion

Important

The type of configuration you pass to this method needs to match the corresponding type that you used to create this display.

If successful, the framework passes the new configuration to the guest, but the guest may or may not respond to parts of the configuration. If the guest doesn’t use the new configuration, the Virtualization framework doesn’t return an error.

Reconfiguration of the display triggers a display state change that you can track by adopting the VZGraphicsDisplayObserver protocol.

## See Also

### Changing the display configuration

func reconfigure(sizeInPixels: CGSize) throws

Resize this display with the new dimensions you provide.

