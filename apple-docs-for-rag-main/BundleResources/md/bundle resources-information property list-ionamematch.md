

- Bundle Resources
- Information Property List
-  IONameMatch 

Property List Key

# IONameMatch

One or more strings that contain the names of possible provider objects in the system registry.

macOS 10.0+

## Details 

Type  

array of strings

## Discussion

The value of this key is a string or an array of strings. The system begins the matching process with a provider object, and looks for additional drivers or nubs that support that provider object. When this key is present, the system compares its values to the provider object’s name. (It also compares the strings to the provider’s `compatible` and `device_type` properties.) If it doesn’t find any matches, the system doesn’t match the driver to the provider object.

The default name of a provider object is its class name, but providers may register a custom name. For more information about how to set or get information for registered services, see IORegistryEntry.

## See Also

### Advanced Match Criteria

IOPropertyMatch

The device-specific keys the system must match in order to use your driver.

IOResourceMatch

One or more system-specific or device-specific resources that your driver requires.

IOParentMatch

IOPathMatch

IOMatchCategory

