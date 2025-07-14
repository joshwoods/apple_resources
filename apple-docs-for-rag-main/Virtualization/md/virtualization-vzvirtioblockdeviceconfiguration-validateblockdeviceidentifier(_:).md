

- Virtualization
- VZVirtioBlockDeviceConfiguration
-  validateBlockDeviceIdentifier(\_:) 

Type Method

# validateBlockDeviceIdentifier(\_:)

Checks the validity of a block device identifier.

macOS 12.3+

``` source
class func validateBlockDeviceIdentifier(_ blockDeviceIdentifier: String) throws
```

## Parameters 

`blockDeviceIdentifier`  

The device identifier to validate. In the case of an invalid identifier string, the method throws an error that describes why the device identifier isn’t valid.

## Discussion

Use validateBlockDeviceIdentifier(_:) to validate an identifier string before trying to set the blockDeviceIdentifier property. The identifier must be an ASCII encodable string of 20 bytes or less.

