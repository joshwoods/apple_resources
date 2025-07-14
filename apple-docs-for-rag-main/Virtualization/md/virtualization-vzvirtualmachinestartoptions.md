

- Virtualization
-  VZVirtualMachineStartOptions 

Class

# VZVirtualMachineStartOptions

The abstract class for VM start options.

macOS 13.0+

``` source
class VZVirtualMachineStartOptions
```

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacOSVirtualMachineStartOptions

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

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

func resume() async throws

Resumes a paused VM and notifies the specified completion handler of the results.

