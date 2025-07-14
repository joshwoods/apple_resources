

- Virtualization
- VZVirtualMachine
-  resume(completionHandler:) 

Instance Method

# resume(completionHandler:)

Resumes a paused VM and notifies the specified completion handler of the results.

macOS 11.0+

``` source
func resume(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

The block to call with the results of the resume attempt. This block has no return value and has one NSError object as its parameter. The completion handler returns an error object when the VM fails to resume.

result  
A result type that contains an error object when the VM fails to resume.

## Discussion

Call this method to resume a VM that’s in the VZVirtualMachine.State.paused state.

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

func pause(completionHandler: (Result&lt;Void, any Error>) -> Void)

Pauses a running VM and notifies the specified completion handler of the results.

func requestStop() throws

Asks the guest operating system to stop running.

func pause() async throws

Pauses a running VM and notifies the specified completion handler of the results.

func resume() async throws

Resumes a paused VM and notifies the specified completion handler of the results.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

