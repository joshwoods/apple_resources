

- Virtualization
- VZVirtioConsolePortConfigurationArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the Virtio console port configuration as the specified index.

macOS 13.0+

``` source
subscript(portIndex: Int) -> VZVirtioConsolePortConfiguration? { get set }
```

## Parameters 

`portIndex`  

The index of the configuration to retrieve.

## Return Value

The VZVirtioConsolePortConfiguration, or nil is the index exceeds the number of configurations in the array.

