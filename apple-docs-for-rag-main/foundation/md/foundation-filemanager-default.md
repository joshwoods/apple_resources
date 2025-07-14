

- Foundation
- FileManager
-  default 

Type Property

# default

The shared file manager object for the process.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: FileManager { get }
```

## Discussion

This method always represents the same file manager object. If you plan to use a delegate with the file manager to receive notifications about the completion of file-based operations, you should create a new instance of FileManager rather than using the shared object.

## See Also

### Creating a File Manager

convenience init(authorization: NSWorkspace.Authorization)

Initializes a file manager object that is authorized to perform privileged file system operations.

