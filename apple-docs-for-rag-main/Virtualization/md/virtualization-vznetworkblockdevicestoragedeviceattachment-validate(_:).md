

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  validate(\_:) 

Type Method

# validate(\_:)

Checks if the URL is a valid network block device URL.

macOS 14.0+

``` source
class func validate(_ URL: URL) throws
```

## Parameters 

`URL`  

The NBD URL to validate.

## Discussion

This method checks that the URL is well-formed; however, it doesn’t attempt to access the URL. See the NBD URL specification on GitHub for more detailed descriptions of valid URIs.

