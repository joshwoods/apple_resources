

- Virtualization
- VZVirtioConsolePortArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the Virtio console port at the specified index.

macOS 13.0+

``` source
subscript(portIndex: Int) -> VZVirtioConsolePort? { get }
```

## Parameters 

`portIndex`  

The index of the port to return, if present.

## Return Value

A VZVirtioConsolePort port, or `nil` if the index is outside the bounds of the array.

