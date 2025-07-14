

- Virtualization
- VZVirtualMachine
-  start(completionHandler:) 

Instance Method

# start(completionHandler:)

Starts the VM and notifies the specified completion handler if startup is successful.

macOS 11.0+

``` source
func start(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

The block to call with the results of the startup attempt. This block has no return value and has one NSError object as its parameter:

result  
A result type that contains an error object when the VM fails to start.

## Discussion

Call this method to start a VM that’s in the VZVirtualMachine.State.stopped or VZVirtualMachine.State.error state. To determine if a VM is in a state that allows you to start it, check the VM’s canStart property.

## See Also

### Starting and stopping the VM

func start() async throws

Starts the VM and notifies the specified completion handler if startup was successful.

func start(options: VZVirtualMachineStartOptions, completionHandler: ((any Error)?) -> Void)

Starts the VM with the options and a completion handler you provide.

func stop(completionHandler: ((any Error)?) -> Void)

Stops a VM that’s in either a running or paused state.

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

