

- Virtualization
-  Creating and Running a Linux Virtual Machine 

Article

# Creating and Running a Linux Virtual Machine

Design and run custom Linux guests on Apple silicon or Intel-based Mac Computers.

## Overview

Running a Linux virtual machine (VM) is an additive process that starts with selecting a Linux distribution and obtaining Linux kernel and RAM disk images, and ends with instantiating and running the Linux VM on the user’s computer.

There many Linux distributions to choose from, select one that both meets your app’s needs in terms of device and application support, and supports ARM64 or 64-bit Intel-based CPUs. You’ll also need to decide how much of the host computer’s CPU resources and memory to dedicate to the VM in order to configure a VZVirtualMachineConfiguration. Unless your VM is solving self-contained computing problems, it’s likely your VM needs to interact with the user, access the network, and so on, so you’ll want to add devices to the VM to make this possible.

Finally, after creating a suitable VZVirtualMachineConfiguration, you’ll use a VZLinuxBootLoader to launch your VM and a VZVirtualMachine instance to control it.

### Obtain the Kernel and RAM Disk Images

You can obtain images for many Linux distributions, including Ubuntu Linux. Most Linux distributions provide downloadable kernel and RAM disk images that can run on Mac computers; however, you’ll need to download images for your specific CPU:

- For Apple silicon Mac computers, download ARM 64-bit images.

- For Intel-based Mac computers, download AMD64 images.

If your app is universal, you’ll need to obtain images for both Apple silicon and Intel-based Mac computers in order to be able to run the appropriate Linux VM on the respective Apple silicon or Intel-based Mac computer.

Note

If the distribution you choose doesn’t provide images for the kernel and RAM disk, you’ll need to assemble and package those images yourself.

Some Linux distributions store kernel images in a compressed format, sometimes indicated by a `.gz` filename extension. If the image doesn’t have a file extension, you can determine the file’s compression status using the `file` command. After determining the file format for the image, add the appropriate filename extension. For example, if the output shows the file format as “gzip compressed data,” add the `.gz` extension to the image, and then use the `gzip` or `gunzip` command to unpack the image. Running `file` against the unpacked image reveals details about the kernel image you’re verifying.

You can include the Linux kernel and RAM disk as resources in your Xcode project for use in your app, or implement a custom solution that allows the user to download and save images over the network.

### Set Up the Linux VM Configuration

Configure a VZVirtualMachineConfiguration with the number of CPUs and amount of memory you want to use with your VM:

- Swift
- Objective-C

```
// Set up global properties.
let virtualMachineConfiguration = VZVirtualMachineConfiguration()
virtualMachineConfiguration.cpuCount = 2
// 2 GB of memory. This is an arbitrary amount.
virtualMachineConfiguration.memorySize = 2 * 1024 * 1024 * 1024 
```

```
// Set up global properties.
VZVirtualMachineConfiguration *virtualMachineConfiguration = [VZVirtualMachineConfiguration new];
virtualMachineConfiguration.CPUCount = 2;
// 2 GB of memory. This is an arbitrary amount.
virtualMachineConfiguration.memorySize = 2 * 1024 * 1024 * 1024;
```

### Add Devices to Your VM

Next, you’ll need to decide what devices your Linux VM needs. Because you can’t change or add devices to a running VM, consider what devices you’ll need to support your app’s use cases and add them to the VM’s configuration. For example, if you need:

- To connect to network services from your VM, add a VZVirtioNetworkDeviceConfiguration.

- A source of entropy, add a VZVirtioEntropyDeviceConfiguration.

- Audio devices, add VZVirtioSoundDeviceOutputStreamConfiguration, VZVirtioSoundDeviceOutputStreamConfiguration, and their associated stream sources and device configurations.

The example below adds a serial console, and sound input and output devices to the VM’s configuration:

- Swift
- Objective-C

```
// Add a serial console and audio devices.
virtualMachineConfiguration.serialPorts = [createConsoleConfiguration()]

let outputStream = VZVirtioSoundDeviceOutputStreamConfiguration()
outputStream.sink = VZHostAudioOutputStreamSink()
let outputSoundDevice = VZVirtioSoundDeviceConfiguration()
outputSoundDevice.streams = [outputStream]

let inputStream = VZVirtioSoundDeviceInputStreamConfiguration()
inputStream.source = VZHostAudioInputStreamSource()
let inputSoundDevice = VZVirtioSoundDeviceConfiguration()
inputSoundDevice.streams = [inputStream]

virtualMachineConfiguration.audioDevices = [outputSoundDevice, inputSoundDevice]
```

```
// Add a serial console and audio devices.
virtualMachineConfiguration.serialPorts = [VMConfigurationHelper createConsoleConfiguration];

VZVirtioSoundDeviceOutputStreamConfiguration *outputStream = [[VZVirtioSoundDeviceOutputStreamConfiguration alloc] init];
outputStream.sink = [[VZHostAudioOutputStreamSink alloc] init];
VZVirtioSoundDeviceConfiguration *outputSoundDevice = [[VZVirtioSoundDeviceConfiguration alloc] init];
soundDevice.streams = @[ outputStream ];

VZVirtioSoundDeviceInputStreamConfiguration *inputStream = [[VZVirtioSoundDeviceInputStreamConfiguration alloc] init];
inputStream.source = [[VZHostAudioInputStreamSource alloc] init];
VZVirtioSoundDeviceConfiguration *inputSoundDevice = [[VZVirtioSoundDeviceConfiguration alloc] init];
soundDevice.streams = @[ inputStream ];

virtualMachineConfiguration.audioDevices = @[ outputSoundDevice, inputSoundDevice ];
```

For more information on devices that Linux guests can support, see the Devices section on the Virtualization framework.

### Create a Boot Loader

Create an instance of a VZLinuxBootLoader on the `VZVirtualMachineConfiguration` with a Linux kernel and a RAM disk that you load from locations on disk:

- Swift
- Objective-C

```
// Set up the boot loader.
let kernelURL = getKernelURL() // URL of the Linux kernel image.
let bootLoader = VZLinuxBootLoader(kernelURL: kernelURL)
bootLoader.initialRamdiskURL = getRamdiskURL()
bootLoader.commandLine = "console=hvc0"
virtualMachineConfiguration.bootLoader = bootLoader

// Validate this configuration against the current hardware;
// exit on error.
try! virtualMachineConfiguration.validate()
```

```
// Set up the boot loader.
NSURL *kernelURL = [VMConfigurationHelper getKernelURL];
VZLinuxBootLoader *bootloader = [[VZLinuxBootLoader alloc] initWithKernelURL: kernelURL];
bootLoader.initialRamdiskURL = [VMConfigurationHelper getRamdiskURL];
bootLoader.commandLine = @"console=hvc0";
virtualMachineConfiguration.bootLoader = bootLoader;

// Validate this configuration against the current hardware;
// exit on error.
assert([virtualMachineConfiguration validateWithError:NULL]);
```

### Instantiate and Run the Linux VM

Instantiate a VZVirtualMachine from the `VZVirtualMachineConfiguration` that you use to start, stop, and control your Linux guest:

- Swift
- Objective-C

```
// Start the VM and check for successful startup when the block returns.
let virtualMachine = VZVirtualMachine(configuration: virtualMachineConfiguration)
virtualMachine.start(completionHandler: { (result) in
    switch result {
    case let .failure(error):
        fatalError("Virtual machine failed to start \(error)")
    default:
        NSLog("Virtual machine successfully started.")
    }
})
```

```
// Start the VM and check for successful startup when the block returns.
VZVirtualMachine *virtualMachine =  [[VZVirtualMachine alloc]   initWithConfiguration:virtualMachineConfiguration];
[VZVirtualMachine startWithCompletionHandler:^(NSError *error)
 {
    if (error) {
        NSLog(@"Virtual machine failed to start \(%@)", error);
        abort();
    }
    NSLog(@"Virtual machine successfully started.");
}];
```

## See Also

### Virtual machine setup

Running macOS in a virtual machine on Apple silicon

Install and run macOS in a virtual machine using the Virtualization framework.

Running Linux in a Virtual Machine

Run a Linux operating system on your Mac using the Virtualization framework.

Running GUI Linux in a virtual machine on a Mac

Install and run GUI Linux in a virtual machine using the Virtualization framework.

Installing macOS on a Virtual Machine

Download a macOS restore image and install it in a new VM.

Virtualize macOS on a Mac

Configure and run macOS guests on Apple silicon.

Virtualize Linux on a Mac

Configure and run Linux guests on Apple silicon and Intel-based Mac computers.

Running Intel Binaries in Linux VMs with Rosetta

Run x86_64 Linux binaries under ARM Linux on Apple silicon.

Accelerating the performance of Rosetta

Improve Rosetta performance by adding support for the total store ordering (TSO) memory model to your Linux kernel.

