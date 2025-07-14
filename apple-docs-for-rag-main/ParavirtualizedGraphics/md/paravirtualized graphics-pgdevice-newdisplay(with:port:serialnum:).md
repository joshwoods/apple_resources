

- Paravirtualized Graphics
- PGDevice
-  newDisplay(with:port:serialNum:) 

Instance Method

# newDisplay(with:port:serialNum:)

Create a display from the specified descriptor and uniquifying parameters.

Mac Catalyst 14.0+macOS 11.0+

``` source
func newDisplay(
    with descriptor: PGDisplayDescriptor,
    port: Int,
    serialNum: UInt32
) -> (any PGDisplay)?
```

**Required**

## Parameters 

`descriptor`  

The description of the new display.

`port`  

The port number on the accelerator for the device to use for the new display. Specify a unique port number for each display.

`serialNum`  

A number that uniquely identifies the display. Ensure that the display persists across multiple launches so that the guest compositor can maintain a consistent display layout.

## Return Value

A new display object, or `nil` if an error occurred.

