

- Foundation
- FileManager
-  changeCurrentDirectoryPath(\_:) 

Instance Method

# changeCurrentDirectoryPath(\_:)

Changes the path of the current working directory to the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func changeCurrentDirectoryPath(_ path: String) -> Bool
```

## Parameters 

`path`  

The path of the directory to which to change.

## Return Value

true if successful, otherwise false.

## Discussion

All relative pathnames refer implicitly to the current working directory.

Warning

This method changes the current working directory for the current process, not just the receiver.

## See Also

### Related Documentation

func fileExists(atPath: String, isDirectory: UnsafeMutablePointer&lt;ObjCBool>?) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func contentsOfDirectory(atPath: String) throws -> [String]

Performs a shallow search of the specified directory and returns the paths of any contained items.

### Managing the Current Directory

var currentDirectoryPath: String

The path to the program’s current directory.

