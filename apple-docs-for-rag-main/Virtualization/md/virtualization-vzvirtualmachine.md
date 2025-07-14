

- Virtualization
-  VZVirtualMachine 

Class

# VZVirtualMachine

An object that manages the overall state and configuration of your VM.

macOS 11.0+

``` source
class VZVirtualMachine
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

Installing macOS on a Virtual Machine

## Overview

A VZVirtualMachine object emulates a complete hardware machine of the same architecture as the underlying Mac computer. Use the VM to execute a guest operating system and any other apps you install. The VM manages the resources that the guest operating system uses, providing access to some hardware resources while emulating others.

Create and configure a VZVirtualMachineConfiguration object with details about how you want to configure your VM, and use that object to create the VZVirtualMachine object. After creating the VM, call the start(completionHandler:) method (Swift) or the start() method (Objective-C) to start the VM and boot the guest operating system.

Important

The creation of a virtual machine requires your app to have the com.apple.security.virtualization entitlement.

## Topics

### Creating the VM

convenience init(configuration: VZVirtualMachineConfiguration)

Creates the VM and configures it with the specified data.

init(configuration: VZVirtualMachineConfiguration, queue: dispatch_queue_t)

Creates and configures the VM with the specified data and dispatch queue.

class var isSupported: Bool

A Boolean value that indicates whether the system supports virtualization.

### Responding to a stopped VM

var delegate: (any VZVirtualMachineDelegate)?

A custom object you use to determine when the VM stops.

protocol VZVirtualMachineDelegate

The methods you use to respond to changes in the state of the VM.

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

class VZVirtualMachineStartOptions

The abstract class for VM start options.

### Configuring VM attributes at runtime

var consoleDevices: [VZConsoleDevice]

The list of configured console devices on the VM.

var memoryBalloonDevices: [VZMemoryBalloonDevice]

The array of devices that you use to adjust the amount of memory available to the guest system.

var networkDevices: [VZNetworkDevice]

The list of configured network devices on the VM.

var socketDevices: [VZSocketDevice]

The array of socket devices that the VM configures for use ports in the guest VM.

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

### Getting the state of the VM

var state: VZVirtualMachine.State

The current execution state of the VM.

enum State

The execution states of the VM.

var graphicsDevices: [VZGraphicsDevice]

The list of configured graphics devices on the virtual machine.

var canStart: Bool

A Boolean value that indicates whether you can start the VM.

var canPause: Bool

A Boolean value that indicates whether you can pause the VM.

var canResume: Bool

A Boolean value that indicates whether you can resume the VM.

var canStop: Bool

A Boolean value that indicates whether you can stop the VM.

var canRequestStop: Bool

A Boolean value that indicates whether you can ask the guest operating system to stop running.

### Saving and restoring the VM state

func saveMachineStateTo(url: URL, completionHandler: ((any Error)?) -> Void)

Saves the state of a VM.

func restoreMachineStateFrom(url: URL, completionHandler: ((any Error)?) -> Void)

Restores a VM from a previously saved state.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Runtime

class VZVirtualMachineView

A view that allows user interaction with a VM.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

