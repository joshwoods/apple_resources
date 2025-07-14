

- Virtualization
- VZGraphicsDisplay
-  reconfigure(sizeInPixels:) 

Instance Method

# reconfigure(sizeInPixels:)

Resize this display with the new dimensions you provide.

macOS 14.0+

``` source
func reconfigure(sizeInPixels: CGSize) throws
```

## Parameters 

`sizeInPixels`  

The new display width and height in pixels.

## Discussion

If successful, the framework passes the new size to the guest but the guest may or may not respond to the new size. If the guest doesn’t use the new size, the Virtualization framework doesn’t return an error.

Resizing the display triggers a display state change that you can track by adopting the VZGraphicsDisplayObserver protocol.

## See Also

### Changing the display configuration

func reconfigure(configuration: VZGraphicsDisplayConfiguration) throws

Reconfigure this display with the new display configuration you provide.

