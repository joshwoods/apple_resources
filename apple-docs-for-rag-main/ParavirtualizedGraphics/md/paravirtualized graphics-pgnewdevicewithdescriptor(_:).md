

- Paravirtualized Graphics
-  PGNewDeviceWithDescriptor(\_:) 

Function

# PGNewDeviceWithDescriptor(\_:)

Creates a new paravirtualized graphics device.

Mac Catalyst 14.0+macOS 11.0+

``` source
func PGNewDeviceWithDescriptor(_ descriptor: PGDeviceDescriptor) -> (any PGDevice)?
```

## Parameters 

`descriptor`  

The configuration to use for the new device.

## Return Value

A new paravirtualized graphics device.

## See Also

### Devices

class PGDeviceDescriptor

A description of the paravirtualized graphics device to create.

protocol PGDevice

A paravirtualized GPU device object.

