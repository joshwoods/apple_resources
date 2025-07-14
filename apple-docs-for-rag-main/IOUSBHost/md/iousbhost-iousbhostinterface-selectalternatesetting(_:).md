

- IOUSBHost
- IOUSBHostInterface
-  selectAlternateSetting(\_:) 

Instance Method

# selectAlternateSetting(\_:)

Selects an alternative setting for the interface.

Mac Catalyst 14.0+macOS 10.15+

``` source
func selectAlternateSetting(_ alternateSetting: Int) throws
```

## Parameters 

`alternateSetting`  

The alternative interface number to activate.

## Discussion

Use this method to select an alternative setting for the interface. The operation aborts all pending input/output requests on the interface’s pipes, and closes all open pipes. It also selects the new alternative setting through the `SET_INTERFACE` control request (See USB 3.2, 9.4.10.).

Note

Any IOUSBHostPipe objects that already exist are no longer valid.

## See Also

### Managing Pipes

func copyPipe(withAddress: Int) throws -> IOUSBHostPipe

Copies a pipe for a specific endpoint address.

