

- Virtualization
- VZVirtualMachine
-  start(options:completionHandler:) 

Instance Method

# start(options:completionHandler:)

Starts the VM with the options and a completion handler you provide.

macOS 13.0+

``` source
func start(
    options: VZVirtualMachineStartOptions,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func start(options: VZVirtualMachineStartOptions) async throws
```

## Parameters 

`options`  

A VZVirtualMachineStartOptions object that describes controlling startup behavior of a VM using VZMacOSBootLoader.

`completionHandler`  

The block to call with the results of the startup attempt. This block has no return value and has one NSError object as its parameter:

error  
A result type that contains an error object when the VM fails to start.

## See Also

### Related Documentation

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

### Starting and stopping the VM

func start(completionHandler: (Result&lt;Void, any Error>) -> Void)

Starts the VM and notifies the specified completion handler if startup is successful.

func start() async throws

Starts the VM and notifies the specified completion handler if startup was successful.

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

