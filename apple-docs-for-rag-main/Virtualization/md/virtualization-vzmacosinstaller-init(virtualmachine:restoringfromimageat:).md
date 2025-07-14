

- Virtualization
- VZMacOSInstaller
-  init(virtualMachine:restoringFromImageAt:) 

Initializer

# init(virtualMachine:restoringFromImageAt:)

Creates a macOS installer object.

macOS 12.0+

``` source
init(
    virtualMachine: VZVirtualMachine,
    restoringFromImageAt restoreImageFileURL: URL
)
```

## Parameters 

`virtualMachine`  

The virtual machine to install the operating system on.

`restoreImageFileURL`  

A file URL that indicates the macOS restore image to install.

