

- Virtualization
- VZVirtualMachine
-  restoreMachineStateFrom(url:completionHandler:) 

Instance Method

# restoreMachineStateFrom(url:completionHandler:)

Restores a VM from a previously saved state.

macOS 14.0+

``` source
func restoreMachineStateFrom(
    url saveFileURL: URL,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func restoreMachineStateFrom(url saveFileURL: URL) async throws
```

## Parameters 

`saveFileURL`  

An NSURL that indicates the location where the framework reads the saved state of the VM.

`completionHandler`  

A block the framework calls after the VM has been successfully restored or upon an error.

## Discussion

Use this method to restore a stopped VM to a state previously saved to file through saveMachineStateTo(url:completionHandler:).

The method fails if any of the following conditions are true:

- The Virtualization framework can’t open or read the file.

- The file contents are incompatible with the current configuration.

- The VM you’re trying to restore isn’t in the VZVirtualMachine.State.stopped state.

If this method fails, the framework returns an error, and the VM state doesn’t change.

If this method is successful, the framework restores the VM and places it in the paused state.

## See Also

### Saving and restoring the VM state

func saveMachineStateTo(url: URL, completionHandler: ((any Error)?) -> Void)

Saves the state of a VM.

