

- Virtualization
- VZSharedDirectory
-  url 

Instance Property

# url

A file URL to a directory on the host system to expose to the guest.

macOS 12.0+

``` source
var url: URL { get }
```

## Discussion

The URL must point to an existing directory path in the host file system.

## See Also

### Accessing Directory Properties

var isReadOnly: Bool

A Boolean value that indicates whether the directory is read-only to the guest.

