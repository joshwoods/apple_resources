

- Virtualization
-  VZVirtualMachineConfiguration 

Class

# VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

macOS 11.0+

``` source
class VZVirtualMachineConfiguration
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

Installing macOS on a Virtual Machine

## Overview

Use a VZVirtualMachineConfiguration object to configure the environment for a macOS or Linux VM. This configuration object contains information about the VM environment, including the devices that the VM exposes to the guest operating system. For example, use the configuration object to specify the network interfaces and storage devices that the operating system may access. For more information on the devices that macOS and Linux guests can support, see the Devices section on the Virtualization framework page.

You create and configure VZVirtualMachineConfiguration objects directly. After validating the configuration object, use it to initialize the VZVirtualMachine object that manages the virtual environment. The smallest valid configuration includes a value for the bootLoader property; you can also include more devices in the configuration depending on the needs of your app, such as graphics devices, shared directories, and so on. When you finish configuring the object, call the validate() method to determine whether a VM can successfully support your configuration. A configuration object is invalid if your app doesn’t have the com.apple.security.virtualization entitlement.

For more information on using `VZVirtualMachineConfiguration`, see Installing macOS on a Virtual Machine and Creating and Running a Linux Virtual Machine.

## Topics

### Configuring the guest system

var bootLoader: VZBootLoader?

The guest system to boot when the VM starts.

### Setting the number of CPUs

var cpuCount: Int

The number of CPUs you make available to the guest operating system.

class var minimumAllowedCPUCount: Int

The minimum number of CPUs you may configure for the VM.

class var maximumAllowedCPUCount: Int

The maximum number of CPUs you may configure for the VM.

### Sizing the memory partition

var memorySize: UInt64

The amount of physical memory the guest operating system recognizes.

class var minimumAllowedMemorySize: UInt64

The minimum amount of memory that you may configure for the VM.

class var maximumAllowedMemorySize: UInt64

The maximum amount of memory that you may configure for the VM.

var memoryBalloonDevices: [VZMemoryBalloonDeviceConfiguration]

An array that you configure with a memory balloon device, used to update the memory in the VM.

### Adding devices to the VM

var consoleDevices: [VZConsoleDeviceConfiguration]

The array of console devices that you expose to the guest operating system.

var networkDevices: [VZNetworkDeviceConfiguration]

The array of network devices that you expose to the guest operating system.

var socketDevices: [VZSocketDeviceConfiguration]

The socket device that you use to implement port-based communication with the guest operating system.

var serialPorts: [VZSerialPortConfiguration]

The array of serial ports that you expose to the guest operating system.

var storageDevices: [VZStorageDeviceConfiguration]

The array of storage devices that you expose to the guest operating system.

var entropyDevices: [VZEntropyDeviceConfiguration]

The array of randomization devices that you expose to the guest operating system.

var audioDevices: [VZAudioDeviceConfiguration]

The list of audio devices.

var directorySharingDevices: [VZDirectorySharingDeviceConfiguration]

The list of directory sharing devices.

var graphicsDevices: [VZGraphicsDeviceConfiguration]

The list of graphics devices.

var keyboards: [VZKeyboardConfiguration]

The list of keyboards.

var platform: VZPlatformConfiguration

The hardware platform to use.

var pointingDevices: [VZPointingDeviceConfiguration]

The list of pointing devices.

var usbControllers: [VZUSBControllerConfiguration]

The list of configured USB controllers for the VM.

### Validating the configuration

func validate() throws

Validates the current configuration settings and reports any issues that might prevent the successful initialization of the VM.

func validateSaveRestoreSupport() throws

Determines whether the framework can save or restore the VM’s current configuration.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZVirtualMachineStartOptions

The abstract class for VM start options.

class VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

class VZPlatformConfiguration

The base class for a platform configuration.

