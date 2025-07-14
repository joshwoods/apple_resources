

- Virtualization
-  VZMacOSInstaller 

Class

# VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

macOS 12.0+

``` source
class VZMacOSInstaller
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Overview

Initialize a VZMacOSInstaller object with a VZVirtualMachine and a file URL that refers to a macOS restore image.

The following code example shows how to use a `VZMacOSInstaller:`

```
// Call VZMacOSInstaller with a URL that corresponds to a local file. 
// This is the storage location for the restore image the app downloads.
let localRestoreImageURL = ...

// Load the latest restore image.
guard let restoreImage = try? await VZMacOSRestoreImage.latestSupported else {
    // Handle the error.
    abort()
}

// Call VZMacOSInstaller with a URL that corresponds to a local file. 
// Because restoreImage came from latestSupported, its URL property refers to a 
// restore image on the network. Download the restore image to the local file system.
guard let (location, _) = try? await URLSession.shared.download(from: restoreImage.url, delegate: nil) 
    else {
        // Handle the error.
        abort()
}

guard ((try? FileManager.default.moveItem(at: location, to: localRestoreImageURL)) != nil) else {
    // Handle the error.
    abort()
}

DispatchQueue.main.async {
    // Becuase this restore image came from VZMacOSRestoreImage.
    // latestSupported, mostFeaturefulSupportedConfiguration should not be nil.
    let configurationRequirements = restoreImage.mostFeaturefulSupportedConfiguration!

    // Construct a VZVirtualMachineConfiguration that satisfies the configuration requirements.
    let configuration = VZVirtualMachineConfiguration()
    configuration.bootLoader = VZMacOSBootLoader()
    configuration.platform = VZMacPlatformConfiguration()

    // The following are minimum values; you can use larger values if desired.
    configuration.cpuCount = configurationRequirements.minimumSupportedCPUCount
    configuration.memorySize = configurationRequirements.minimumSupportedMemorySize

    // Set other configuration properties as necessary.
    // ...

guard ((try? configuration.validate()) != nil) else {
    // Handle the error.
    abort()
}

let virtualMachine = VZVirtualMachine(configuration: configuration)
let installer = VZMacOSInstaller(virtualMachine: virtualMachine, restoringFromImageAt: localRestoreImageURL)
installer.install(completionHandler: { (result: Result) in
    if case let .failure(error) = result {
        // Handle the error.
        abort()
    } else {
        // Installation was successful.
    }
})

// Observe progress using installer.progress object.
}
```

## Topics

### Creating a macOS Installer

init(virtualMachine: VZVirtualMachine, restoringFromImageAt: URL)

Creates a macOS installer object.

### Getting Information About an Installation

var progress: Progress

A progress object that you can use to observe or cancel an installation.

var restoreImageURL: URL

The restore image URL used to initialize this installer.

var virtualMachine: VZVirtualMachine

The virtual machine used to initialize this installer.

### Installing macOS

func install(completionHandler: (Result&lt;Void, any Error>) -> Void)

Start installing macOS.

func install() async throws

Start installing macOS.

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

### Related Documentation

class VZVirtualMachine

An object that manages the overall state and configuration of your VM.

### Installers

class VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

class VZMacOSConfigurationRequirements

An object that describes the parameter constraints required by a specific configuration of macOS.

