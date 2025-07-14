

- Virtualization
-  Running Intel Binaries in Linux VMs with Rosetta 

Article

# Running Intel Binaries in Linux VMs with Rosetta

Run x86_64 Linux binaries under ARM Linux on Apple silicon.

## Overview

In macOS 13 and later on Mac computers with Apple silicon chips, the Virtualization framework supports Rosetta in ARM Linux virtual machines (VMs). Rosetta is a translation process that allows users to run apps that contain x86_64 instructions on Apple silicon. In macOS, this allows apps built for Intel-based Mac computers to run seamlessly on Apple silicon; Rosetta allows the same capability for Intel Linux apps in ARM Linux VMs.

Note

Rosetta doesn’t support the bootstrapping or installation of Intel Linux distributions on Mac computers with Apple silicon using the Virtualization framework. Intel Linux distributions can run using the Virtualization framework on Intel-based Mac computers without the need for this translation capability.

### Test for Rosetta Availability

Before trying to install, run, or activate Rosetta, your app should check to ensure that the capability is available in the version of macOS running on the host computer. The availability class method returns a value from the VZLinuxRosettaAvailability enumeration that describes whether the current host supports Rosetta or if the capability is already installed on the host Mac. The example below shows the process for checking for Rosetta availability:

- Swift
- Objective-C

```
import Virtualization

let rosettaAvailability = VZLinuxRosettaDirectoryShare.availability

switch rosettaAvailability {
case notSupported:
    // Alert the user the capability isn't available; offer 
    // continuation options according to your app's requirements.

case notInstalled:
    // Ask the user for permission to install Rosetta, and 
    // start the installation process if they grant permission.

case installed:
    break // Ready to go.
}
```

```
import 

VZLinuxRosettaAvailability rosettaAvailability = VZLinuxRosettaDirectoryShare.availability;
switch (rosettaAvailability) {
    case VZLinuxRosettaAvailabilityNotSupported:
        // Alert the user the capability isn't available; offer 
        // continuation options according to your app's requirements.

    case VZLinuxRosettaAvailabilityNotInstalled:
        // Ask the user for permission to install Rosetta, and 
        // start the installation process if they grant permission.

    case VZLinuxRosettaAvailabilityInstalled:
        break; // Ready to go.
}
```

### Install Rosetta

Installing Rosetta is a one-time process per computer that requires the user to grant permission for the system to install Rosetta. If Rosetta is already installed in macOS, the system activates it for use under the Virtualization framework; if Rosetta isn’t installed, the framework downloads the installer from the network and performs the installation. The installer interactively prompts the user for authorization, and your app should handle any of the possible error conditions that could occur during the authorization, download, and installation process. The example below shows how to start the installation:

- Swift
- Objective-C

```
do {
    try await VZLinuxRosettaDirectoryShare.installRosetta()
    // Success: The system installs Rosetta on the host system.
} catch let error {
    switch error.code {
    case networkError:
        // A network error prevented the download from completing successfully.
    case outOfDiskSpace:
        // Not enough disk space on the system volume to complete the installation.
    case userCancelled:
        // The user cancelled the installation.
    case notSupported:
        // Rosetta isn't supported on the host Mac or macOS version.

    default:
        break // A non installer-related error occurred.
    }
}
```

```
[VZLinuxRosettaDirectoryShare installRosettaWithCompletionHandler:^(NSError *error) {
    if (!error) {
        // Success: The system installs Rosetta on the host system.
    } else {
        // Handle error if error is not nil:
        switch error.code {
             case VSErrorNetworkError:
                 // A network error prevented the download from completing successfully.
             case VZErrorOutOfDiskSpace:
                 // Not enough disk space on the system volume to complete the installation.
             case VZErrorUserCancelled:
                 // The user cancelled the installation.
             case VZErrorNotSupported:
                // Rosetta isn't supported on the host Mac or macOS version.
            default:
               break; // A non installer-related error occurred.
        }
    }
}];
```

### Create the Rosetta Directory Share

After installing Rosetta, your app needs to configure a Rosetta directory share in the Linux guest. The shared directory must have a tag that uniquely identifies the share and that you validate using validateTag(_:) to ensure it conforms to the length and format for file system tags:

- Swift
- Objective-C

```
let tag = "EXAMPLE_TAG"  
let configuration = VZVirtualMachineConfiguration()
do {
    try let validationError = VZVirtioFileSystemDeviceConfiguration.validateTag(tag)
    let rosettaDirectoryShare = try VZLinuxRosettaDirectoryShare()
    let fileSystemDevice = VZVirtioFileSystemDeviceConfiguration(tag: tag)
    fileSystemDevice.share = rosettaDirectoryShare

    configuration.directorySharingDevices = [ fileSystemDevice ]
} catch VZError.invalidVirtualMachineConfiguration {
    // Rosetta is unavailable.
}
```

```
NSString *tag = @"EXAMPLE_TAG";
NSError *validationError = [[VZVirtioFileSystemDeviceConfiguration] validateTag: tag];
if (validationError) {
    AbortWithErrorMessage("Tag %@", tag.localizedDescription); // tag failed to validate.
}

VZVirtualMachineConfiguration *configuration = [[VZVirtualMachineConfiguration alloc] init];
VZVirtioFileSystemDeviceConfiguration *fileSystemDevice = [[VZVirtioFileSystemDeviceConfiguration alloc] initWithTag:tag];

NSError *error = nil;
VZLinuxRosettaDirectoryShare *rosettaDirectoryShare = [[VZLinuxRosettaDirectoryShare alloc] initWithError:&error];
if (rosettaDirectoryShare) {
    fileSystemDevice.share = rosettaDirectoryShare;
    configuration.directorySharingDevices = @[ fileSystemDevice ];
} else {
    // Rosetta is unavailable.
}
```

### Mount the Shared Directory and Register Rosetta

In order to use Rosetta in the Linux guest, the user must mount the Rosetta share in the guest VM and install Rosetta as the application the system uses to run x86_64 binaries using the following process:

Important

The remaining steps required to activate Rosetta in a Linux guest aren’t commands that your app can execute or that you can script from inside your application to a Linux VM; the user must perform them either interactively or as part of a script while logged in to the Linux guest. You must communicate these requirements to the user of your app.

1.  Install the `update-binfmts` command, if necessary. The command is part of the binfmt-support package in most Linux distributions; installation methods vary by distribution. Additionally, in order to run this command, the user must be able to use the `sudo` command, which requires adding their username to the system’s `/etc/sudoers` file.

2.  Create a directory as a mount point.

3.  Mount the VirtioFS file system tag to the mount point. This is the file system tag the app uses to identify the share and must be the same as the tag the user specifies on the command line demonstrated here.

4.  Check if the mounted directory has the Rosetta runtime. You should see `rosetta` in the mounted directory.

5.  Register the Rosetta runtime binary as the handler for x86_64 ELF format executable files using the `update-binfmts` command. The `magic` parameter describes the first 20 bytes of the ELF header for x86_64 binaries. The Linux kernel performs a bitwise logical `AND` with the first 20 bytes of a binary a user attempts to run with the `mask` value. If it matches the `magic` value, the kernel uses the registered handler as the interpreter for that binary. If the system can’t find a handler for the specified binary, it reports an error.

The example below lists the commands, with the exception of the `update-binfmts` command installation, required to enable Rosetta in the Linux guest:

Important

When using Rosetta in macOS 13, set the `preserve` option to `no.`

```
```

### Ensure Shared Libraries are Available for Dynamically Linked Apps

Rosetta can run statically linked x86_64 binaries without additional configuration. Binaries that are dynamically linked and that depend on shared libraries require the installation of the shared libraries, or library hierarchies, in the Linux guest in paths that are accessible to both the user and to Rosetta.

### Configure Rosetta’s ahead of time (AOT) caching options

In macOS 14 and later, Rosetta supports options that allow you control the ahead of time (AOT) cache characteristics; this can improve the performance of some X86 workloads.

There are two modes of operation for AOT caching: The first is communication using a Unix Domain Socket where the Virtualization framework shares a file that represents the socket between the Rosetta daemon and Rosetta runtime through a symlink or bind-mount. The second is communication through an abstract socket where the framework defines a shared name rather than a shared file. 

You enable these options after you create the Rosetta directory share by setting one of the VZLinuxRosettaDirectoryShare.CachingOptions using setCachingOptions(_:). This example shows how to configure Rosetta’s caching options in a new virtual machine configuration using a Unix Domain Socket though a shared, named file:

- Swift
- Objective-C

```
    let configuration = VZVirtualMachineConfiguration()
    do {
        let rosettaDirectoryShare = try VZLinuxRosettaDirectoryShare()
        try rosettaDirectoryShare.setCachingOptions(cachingOptions: .unixSocket("/valid/path/rosetta.sock"))

        let fileSystemDevice = VZVirtioFileSystemDeviceConfiguration(tag: "example-tag")
        fileSystemDevice.share = rosettaDirectoryShare

        configuration.directorySharingDevices = [ fileSystemDevice ]
    } catch VZError.invalidVirtualMachineConfiguration {
        // Rosetta for Linux is unavailable or failed to initialize Rosetta caching options.
        // If Rosetta for Linux is unavailable, clients may install the resources or proceed without them.
        // If Rosetta caching options failed to initialize, clients may gracefully fail or proceed without caching.
    }
```

```
    VZVirtualMachineConfiguration *configuration = [[VZVirtualMachineConfiguration alloc] init];
    VZVirtioFileSystemDeviceConfiguration *fileSystemDevice = [[VZVirtioFileSystemDeviceConfiguration alloc] initWithTag:@"example-tag"];

    NSError *error = nil;
    VZLinuxRosettaDirectoryShare *rosettaDirectoryShare = [[VZLinuxRosettaDirectoryShare alloc] initWithError:&error];
    if (rosettaDirectoryShare) {
        error = nil;
        VZLinuxRosettaUnixSocketCachingOptions *rosettaCachingOptions = [[VZLinuxRosettaUnixSocketCachingOptions alloc] initWithPath:@"/valid/path/rosetta.sock" error:&error];
        if (rosettaCachingOptions) {
            rosettaDirectoryShare.options = rosettaCachingOptions;
            fileSystemDevice.share = rosettaDirectoryShare;
            configuration.directorySharingDevices = @[ fileSystemDevice ];
        } else {
            // Failed to initialize Rosetta caching options. Clients may gracefully fail or proceed without caching.
        }
    } else {
        // Rosetta for Linux is unavailable. Clients may install the resources or proceed without them.
    }
```

The following example shows how to configure Rosetta’s caching options in a new virtual machine configuration using an abstract socket:

- Swift
- Objective-C

```
    let configuration = VZVirtualMachineConfiguration()
    do {
        let rosettaDirectoryShare = try VZLinuxRosettaDirectoryShare()
        try rosettaDirectoryShare.setCachingOptions(.abstractSocket("abstractSocketName"))

        let fileSystemDevice = VZVirtioFileSystemDeviceConfiguration(tag: "example-tag")
        fileSystemDevice.share = rosettaDirectoryShare

        configuration.directorySharingDevices = [ fileSystemDevice ]
    } catch VZError.invalidVirtualMachineConfiguration {
        // Rosetta for Linux is unavailable or failed to initialize Rosetta caching options.
        // If Rosetta for Linux is unavailable, clients may install the resources or proceed without them.
        // If Rosetta caching options failed to initialize, clients may gracefully fail or proceed without caching.
    }    
```

```
    VZVirtualMachineConfiguration *configuration = [[VZVirtualMachineConfiguration alloc] init];
    VZVirtioFileSystemDeviceConfiguration *fileSystemDevice = [[VZVirtioFileSystemDeviceConfiguration alloc] initWithTag:@"example-tag"];

    NSError *error = nil;
    VZLinuxRosettaDirectoryShare *rosettaDirectoryShare = [[VZLinuxRosettaDirectoryShare alloc] initWithError:&error];
    if (rosettaDirectoryShare) {
        VZLinuxRosettaAbstractSocketCachingOptions *options = [[VZLinuxRosettaAbstractSocketCachingOptions alloc] initWithName:@"abstractSocketName" error:&error];
        if (rosettaCachingOptions) {
            rosettaDirectoryShare.options = rosettaCachingOptions;
            fileSystemDevice.share = rosettaDirectoryShare;
            configuration.directorySharingDevices = @[ fileSystemDevice ];
        } else {
            // Failed to initialize Rosetta caching options. Clients may gracefully fail or proceed without caching.
        }
       } else {
        // Rosetta for Linux is unavailable. Clients may install the resources or proceed without them.
    }
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

Creating and Running a Linux Virtual Machine

Design and run custom Linux guests on Apple silicon or Intel-based Mac Computers.

Virtualize macOS on a Mac

Configure and run macOS guests on Apple silicon.

Virtualize Linux on a Mac

Configure and run Linux guests on Apple silicon and Intel-based Mac computers.

Accelerating the performance of Rosetta

Improve Rosetta performance by adding support for the total store ordering (TSO) memory model to your Linux kernel.

