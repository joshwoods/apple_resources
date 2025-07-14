

- Virtualization
- VZLinuxRosettaDirectoryShare
- VZLinuxRosettaDirectoryShare.CachingOptions
-  VZLinuxRosettaDirectoryShare.CachingOptions.unixSocket(\_:) 

Case

# VZLinuxRosettaDirectoryShare.CachingOptions.unixSocket(\_:)

The value that describes an UNIX domain socket at a path that you specify.

macOS 14.0+

``` source
case unixSocket(String)
```

## Parameters 

`path`  

The path of the Unix Domain Socket for Rosetta to use.

## Discussion

Important

The guest operating system needs to have a directory at `path` created in order for translation caching to operate correctly.

## See Also

### Socket types

case abstractSocket(String)

The value that describes an abstract socket with a name you specify.

