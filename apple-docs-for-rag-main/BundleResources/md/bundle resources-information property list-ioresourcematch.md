

- Bundle Resources
- Information Property List
-  IOResourceMatch 

Property List Key

# IOResourceMatch

One or more system-specific or device-specific resources that your driver requires.

macOS 10.0+

## Details 

Type  

string

## Discussion

The value of this key is a string or an array of strings. Each string contains the name of a resource that must be published in the global resource list before the system loads the driver. For example, specify `IOBSD` to prevent the system from loading your driver until after the BSD kernel is available.

To access the list of global resources, call the getResourceService method of IOService. To publish custom resources from your driver, call the publishResource method.

## See Also

### Advanced Match Criteria

IOPropertyMatch

The device-specific keys the system must match in order to use your driver.

IONameMatch

One or more strings that contain the names of possible provider objects in the system registry.

IOParentMatch

IOPathMatch

IOMatchCategory

