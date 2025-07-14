

- Virtualization
- VZLinuxBootLoader
-  init(kernelURL:) 

Initializer

# init(kernelURL:)

Creates a boot loader that launches the Linux kernel at the specified URL.

macOS 11.0+

``` source
init(kernelURL: URL)
```

## Parameters 

`kernelURL`  

The location of a Linux kernel on the local file system.

## Return Value

A boot loader object for the specified Linux kernel.

