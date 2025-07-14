

- Virtualization
- VZVirtioFileSystemDeviceConfiguration
-  init(tag:) 

Initializer

# init(tag:)

Creates a configuration for a VIRTIO file system device.

macOS 12.0+

``` source
init(tag: String)
```

## Parameters 

`tag`  

The label identifying this device in the guest.

## Discussion

The system presents the `tag` as a label in the guest identifying this device for mounting. The `tag` must be valid, which you can check with validateTag(_:).

## See Also

### Related Documentation

class func validateTag(String) throws

Checks to see whether a Virtio tag is valid.

