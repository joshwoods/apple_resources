

- Virtualization
- VZVirtualMachine
-  pause(completionHandler:) 

Instance Method

# pause(completionHandler:)

Pauses a running VM and notifies the specified completion handler of the results.

macOS 11.0+

``` source
func pause(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

The block to call with the results of the pause attempt. This block has no return value and has one NSError object as its parameter:

result  
A result type that contains an error object when the VM fails to pause.

## Discussion

Call this method to pause a Vm that’s in the VZVirtualMachine.State.running state. To determine if a virtual machine is in a state that allows you to pause it, check the VM’s canPause property.

## See Also

### Starting and stopping the VM

func start(completionHandler: (Result&lt;Void, any Error>) -> Void)

Starts the VM and notifies the specified completion handler if startup is successful.

func start() async throws

Starts the VM and notifies the specified completion handler if startup was successful.

func start(options: VZVirtualMachineStartOptions, completionHandler: ((any Error)?) -> Void)

Starts the VM with the options and a completion handler you provide.

func stop(completionHandler: ((any Error)?) -> Void)

Stops a VM that’s in either a running or paused state.

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

