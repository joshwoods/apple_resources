

- Foundation
- FileManager
-  init(authorization:) 

Initializer

# init(authorization:)

Initializes a file manager object that is authorized to perform privileged file system operations.

macOS 10.14+

``` source
convenience init(authorization: NSWorkspace.Authorization)
```

## See Also

### Creating a File Manager

class var `default`: FileManager

The shared file manager object for the process.

