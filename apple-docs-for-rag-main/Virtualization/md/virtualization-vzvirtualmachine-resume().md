

- Virtualization
- VZVirtualMachine
-  resume() 

Instance Method

# resume()

Resumes a paused VM and notifies the specified completion handler of the results.

macOS 11.0+

``` source
func resume() async throws
```

## Discussion

Call this method to resume a VM that’s in the VZVirtualMachine.State.paused state. To determine if a VM is in a state that allows you to resume it, check the VM’s canResume property.

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

func resume(completionHandler: (Result&lt;Void, any Error>) -> Void)

Resumes a paused VM and notifies the specified completion handler of the results.

func pause() async throws

Pauses a running VM and notifies the specified completion handler of the results.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

