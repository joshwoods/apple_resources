

- Virtualization
- VZLinuxBootLoader
-  initialRamdiskURL 

Instance Property

# initialRamdiskURL

The location of an optional RAM disk, which the boot loader maps into memory before it boots the Linux kernel.

macOS 11.0+

``` source
var initialRamdiskURL: URL? { get set }
```

## Discussion

The default value of this property is `nil`. If you want specific files to be available when your Linux kernel boots, provide a URL to a valid RAM disk file in this property.

## See Also

### Configuring the boot parameters

var commandLine: String

The command-line parameters to pass to the Linux kernel at boot time.

