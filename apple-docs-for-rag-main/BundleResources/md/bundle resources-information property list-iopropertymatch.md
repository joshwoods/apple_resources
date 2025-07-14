

- Bundle Resources
- Information Property List
-  IOPropertyMatch 

Property List Key

# IOPropertyMatch

The device-specific keys the system must match in order to use your driver.

macOS 10.0+

## Details 

Type  

object

## Discussion

The value of this key is a dictionary of device-specific keys and values to use during the matching process. For the system to match the driver personality to a device, all keys in the dictionary must be present in the device, and all values must exactly match the device-provided values.

## See Also

### Advanced Match Criteria

IONameMatch

One or more strings that contain the names of possible provider objects in the system registry.

IOResourceMatch

One or more system-specific or device-specific resources that your driver requires.

IOParentMatch

IOPathMatch

IOMatchCategory

