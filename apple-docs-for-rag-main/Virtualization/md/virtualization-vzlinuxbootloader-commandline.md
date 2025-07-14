

- Virtualization
- VZLinuxBootLoader
-  commandLine 

Instance Property

# commandLine

The command-line parameters to pass to the Linux kernel at boot time.

macOS 11.0+

``` source
var commandLine: String { get set }
```

## Discussion

For information about the parameters you can pass to a Linux kernel, see “The kernel’s command-line parameters”.

## See Also

### Configuring the boot parameters

var initialRamdiskURL: URL?

The location of an optional RAM disk, which the boot loader maps into memory before it boots the Linux kernel.

