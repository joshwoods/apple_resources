

- Virtualization
- VZLinuxRosettaDirectoryShare
-  init() 

Initializer

# init()

Creates a new Rosetta directory share, or returns an error if Rosetta isn’t installed.

macOS 13.0+

``` source
init() throws
```

## Discussion

Check the status of Rosetta by examining the availability class property before creating a new Rosetta directory share to ensure the capability is both supported and available on host Mac. For complete instructions on installing Rosetta see Running Intel Binaries in Linux VMs with Rosetta.

