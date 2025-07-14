

- Virtualization
- VZMultipleDirectoryShare
-  directories 

Instance Property

# directories

The directories on the host to expose to the guest.

macOS 12.0+

``` source
var directories: [String : VZSharedDirectory] { get }
```

## Discussion

The dictionary string keys are the names for the directory. The keys must be valid names or the system raises an exception.

## See Also

### Related Documentation

class func validateName(String) throws

Check if a name is a valid directory name.

