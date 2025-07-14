

- IOBluetooth
- OBEXFileTransferServices
-  isBusy() 

Instance Method

# isBusy()

Get the action state of the module

macOS

``` source
func isBusy() -> Bool
```

## Return Value

Success or failure code.

## Discussion

OBEXFileTransferServices will be considered “busy” when an operation in taking place or has not completed. Calling abort: on this module will not automatically reset its busy state. The user will have to wait for the operation to complete or for the current operation to timeout.

