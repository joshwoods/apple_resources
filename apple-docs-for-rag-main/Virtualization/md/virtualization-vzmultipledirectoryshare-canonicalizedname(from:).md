

- Virtualization
- VZMultipleDirectoryShare
-  canonicalizedName(from:) 

Type Method

# canonicalizedName(from:)

Transforms a string to be a valid directory name.

macOS 12.0+

``` source
class func canonicalizedName(from name: String) -> String?
```

## Parameters 

`name`  

The name to transform.

## Return Value

Returns a String with the canonicalized name, or `nil` if there was an error.

## See Also

### Directory name utility methods

class func validateName(String) throws

Check if a name is a valid directory name.

