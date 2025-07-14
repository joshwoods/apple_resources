

- Virtualization
- VZVirtualMachine
-  stop(completionHandler:) 

Instance Method

# stop(completionHandler:)

Stops a VM that’s in either a running or paused state.

macOS 12.0+

``` source
func stop(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func stop() async throws
```

## Parameters 

`completionHandler`  

A block called after the VM stopped successfully, or on error. The error parameter passed to the block is `nil` if the stop was successful.

## Discussion

Warning

This is a destructive operation. It stops the VM without giving the guest a chance to stop cleanly.

To determine if a VM is in a state that allows you to stop it, check the VM’s canStop or canRequestStop properties.

## See Also

### Starting and stopping the VM

func start(completionHandler: (Result&lt;Void, any Error>) -> Void)

Starts the VM and notifies the specified completion handler if startup is successful.

func start() async throws

Starts the VM and notifies the specified completion handler if startup was successful.

func start(options: VZVirtualMachineStartOptions, completionHandler: ((any Error)?) -> Void)

Starts the VM with the options and a completion handler you provide.

func pause(completionHandler: (Result&lt;Void, any Error>) -> Void)

Pauses a running VM and notifies the specified completion handler of the results.

func requestStop() throws

Asks the guest operating system to stop running.

func resume(completionHandler: (Result&lt;Void, any Error>) -> Void)

Resumes a paused VM and notifies the specified completion handler of the results.

func pause() async throws

Pauses a running VM and notifies the specified completion handler of the results.

func resume() async throws

Resumes a paused VM and notifies the specified completion handler of the results.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

