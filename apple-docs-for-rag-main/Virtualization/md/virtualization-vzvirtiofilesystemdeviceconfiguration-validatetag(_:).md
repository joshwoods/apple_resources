

- Virtualization
- VZVirtioFileSystemDeviceConfiguration
-  validateTag(\_:) 

Type Method

# validateTag(\_:)

Checks to see whether a Virtio tag is valid.

macOS 12.0+

``` source
class func validateTag(_ tag: String) throws
```

## Parameters 

`tag`  

The tag to validate.

## Mentioned in 

Running Intel Binaries in Linux VMs with Rosetta

## Discussion

The tag can’t be empty and must be fewer than 36 bytes when encoded in UTF-8.

