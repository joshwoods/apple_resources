

- Virtualization
- VZLinuxRosettaDirectoryShare
-  setCachingOptions(\_:) 

Instance Method

# setCachingOptions(\_:)

Sets the Rosetta caching options using the options you specify.

macOS 14.0+

``` source
func setCachingOptions(_ cachingOptions: VZLinuxRosettaDirectoryShare.CachingOptions?) throws
```

## Parameters 

`cachingOptions`  

One of the available VZLinuxRosettaDirectoryShare.CachingOptions.

## Mentioned in 

Running Intel Binaries in Linux VMs with Rosetta

## See Also

### Setting the ahead of time (AOT) caching options

var cachingOptions: VZLinuxRosettaDirectoryShare.CachingOptions?

The value that enables translation caching and configures the socket communication type for Rosetta.

enum CachingOptions

Socket values you specify to configure Rosetta’s caching capabilities.

