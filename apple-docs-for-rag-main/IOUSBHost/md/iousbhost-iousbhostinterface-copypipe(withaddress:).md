

- IOUSBHost
- IOUSBHostInterface
-  copyPipe(withAddress:) 

Instance Method

# copyPipe(withAddress:)

Copies a pipe for a specific endpoint address.

Mac Catalyst 14.0+macOS 10.15+

``` source
func copyPipe(withAddress address: Int) throws -> IOUSBHostPipe
```

## Parameters 

`address`  

The endpoint address of the pipe.

## Return Value

An IOUSBHostPipe or nil if the system can’t create the pipe.

## Discussion

If the pipe returns successfully, the method maintains a reference to the IOUSBHostInterface.

## See Also

### Managing Pipes

func selectAlternateSetting(Int) throws

Selects an alternative setting for the interface.

