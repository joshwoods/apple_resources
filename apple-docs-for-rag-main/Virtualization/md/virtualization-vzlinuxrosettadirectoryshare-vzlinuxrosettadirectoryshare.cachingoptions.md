

- Virtualization
- VZLinuxRosettaDirectoryShare
-  VZLinuxRosettaDirectoryShare.CachingOptions 

Enumeration

# VZLinuxRosettaDirectoryShare.CachingOptions

Socket values you specify to configure Rosetta’s caching capabilities.

macOS 14.0+

``` source
enum CachingOptions
```

## Mentioned in 

Running Intel Binaries in Linux VMs with Rosetta

## Topics

### Socket types

case abstractSocket(String)

The value that describes an abstract socket with a name you specify.

case unixSocket(String)

The value that describes an UNIX domain socket at a path that you specify.

### Type properties

static var defaultUnixSocket: VZLinuxRosettaDirectoryShare.CachingOptions

The options to use for a default UNIX domain socket.

static var maximumNameLength: Int

The maximum length of the name of an abstract socket.

static var maximumPathLength: Int

The maximum length of the path to a UNIX domain socket.

## See Also

### Setting the ahead of time (AOT) caching options

var cachingOptions: VZLinuxRosettaDirectoryShare.CachingOptions?

The value that enables translation caching and configures the socket communication type for Rosetta.

func setCachingOptions(VZLinuxRosettaDirectoryShare.CachingOptions?) throws

Sets the Rosetta caching options using the options you specify.

