

- Foundation
- FileManager
-  currentDirectoryPath 

Instance Property

# currentDirectoryPath

The path to the program’s current directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currentDirectoryPath: String { get }
```

## Discussion

The current directory path is the starting point for any relative paths you specify. For example, if the current directory is `/tmp` and you specify a relative pathname of `reports/info.txt`, the resulting full path for the item is `/tmp/reports/info.txt`.

When an app is launched, this property is initially set to the app’s current working directory. If the current working directory is not accessible for any reason, the value of this property is `nil`. You can change the value of this property by calling the changeCurrentDirectoryPath(_:) method.

Warning

This property reports the current working directory for the current process, not just the receiver.

## See Also

### Related Documentation

func createDirectory(atPath: String, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with given attributes at the specified path.

### Managing the Current Directory

func changeCurrentDirectoryPath(String) -> Bool

Changes the path of the current working directory to the specified path.

