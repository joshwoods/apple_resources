

- Virtualization
- VZMultipleDirectoryShare
-  init(directories:) 

Initializer

# init(directories:)

Creates the directory share with a set of directories on the host.

macOS 12.0+

``` source
init(directories: [String : VZSharedDirectory])
```

## Parameters 

`directories`  

Directories on the host to expose to the guest VM by name.

## Discussion

The dictionary string keys are the names for the directory. The keys must be valid names or the system raises an exception and the app exits.

## See Also

### Related Documentation

class func validateName(String) throws

Check if a name is a valid directory name.

### Creating a directory share

convenience init()

Initializes the directory share with an empty set of directories.

