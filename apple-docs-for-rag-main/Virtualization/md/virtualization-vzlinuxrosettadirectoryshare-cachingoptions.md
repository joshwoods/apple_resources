

- Virtualization
- VZLinuxRosettaDirectoryShare
-  cachingOptions 

Instance Property

# cachingOptions

The value that enables translation caching and configures the socket communication type for Rosetta.

macOS 14.0+

``` source
var cachingOptions: VZLinuxRosettaDirectoryShare.CachingOptions? { get }
```

## See Also

### Setting the ahead of time (AOT) caching options

func setCachingOptions(VZLinuxRosettaDirectoryShare.CachingOptions?) throws

Sets the Rosetta caching options using the options you specify.

enum CachingOptions

Socket values you specify to configure Rosetta’s caching capabilities.

