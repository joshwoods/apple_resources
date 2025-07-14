

- Virtualization
- VZMacOSInstaller
-  progress 

Instance Property

# progress

A progress object that you can use to observe or cancel an installation.

macOS 12.0+

``` source
var progress: Progress { get }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

Canceling the progress object before starting an installation raises an exception.

## See Also

### Getting Information About an Installation

var restoreImageURL: URL

The restore image URL used to initialize this installer.

var virtualMachine: VZVirtualMachine

The virtual machine used to initialize this installer.

