

- Virtualization
- VZMacGraphicsDisplayConfiguration
-  init(for:sizeInPoints:) 

Initializer

# init(for:sizeInPoints:)

Create a display configuration suitable for showing on the specified screen.

macOS 12.0+

``` source
convenience init(
    for screen: NSScreen,
    sizeInPoints: NSSize
)
```

## Parameters 

`screen`  

The screen on which you intend to present the VZVirtualMachineView for the display.

`sizeInPoints`  

The intended logical size of the display.

## Discussion

The framework initializes the pixel dimensions and pixel density based on the specified screen and size. An instance of macOS running in the VM may not necessarily provide a display mode with a backing scale factor matching the specified screen.

## See Also

### Creating the display configuration

init(widthInPixels: Int, heightInPixels: Int, pixelsPerInch: Int)

Create a display configuration with the specified pixel dimensions and pixel density.

