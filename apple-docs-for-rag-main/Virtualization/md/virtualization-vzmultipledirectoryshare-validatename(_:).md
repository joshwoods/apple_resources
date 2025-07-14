

- Virtualization
- VZMultipleDirectoryShare
-  validateName(\_:) 

Type Method

# validateName(\_:)

Check if a name is a valid directory name.

macOS 12.0+

``` source
class func validateName(_ name: String) throws
```

## Parameters 

`name`  

The name to validate.

## Discussion

The name must not be empty, have characters unsafe for file systems, be longer than `NAME_MAX`, or using a reserved name such as the Unix “.” or “..” current and parent directory filenames.

## See Also

### Directory name utility methods

class func canonicalizedName(from: String) -> String?

Transforms a string to be a valid directory name.

