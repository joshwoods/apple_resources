

- IOUSBHost
- IOUSBHostDevice
-  configurationDescriptor 

Instance Property

# configurationDescriptor

The currently selected configuration descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
var configurationDescriptor: UnsafePointer? { get }
```

## Return Value

A pointer to the device’s configuration descriptor, or `nil` if no matching descriptor returns.

## Discussion

Note

The IOUSBHostDevice performs memory management. Don’t free the descriptor, and assume it is valid as long as the IOUSBHostDevice hasn’t called destroy().

