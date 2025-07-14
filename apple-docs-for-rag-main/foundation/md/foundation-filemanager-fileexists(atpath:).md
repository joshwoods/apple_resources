

- Foundation
- FileManager
-  fileExists(atPath:) 

Instance Method

# fileExists(atPath:)

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fileExists(atPath path: String) -> Bool
```

## Parameters 

`path`  

The path of the file or directory. If `path` begins with a tilde (`~`), it must first be expanded with expandingTildeInPath; otherwise, this method returns false.

App Sandbox does not restrict which path values may be passed to this parameter.

## Return Value

true if a file at the specified path exists, or false if the file does not exist or its existence could not be determined.

## Discussion

If the file at `path` is inaccessible to your app, perhaps because one or more parent directories are inaccessible, this method returns false. If the final element in `path` specifies a symbolic link, this method traverses the link and returns true or false based on the existence of the file at the link destination.

Note

Attempting to predicate behavior based on the current state of the file system or a particular file on the file system is not recommended. Doing so can cause odd behavior or race conditions. It’s far better to attempt an operation (such as loading a file or creating a directory), check for errors, and handle those errors gracefully than it is to try to figure out ahead of time whether the operation will succeed. For more information on file-system race conditions, see Race Conditions and Secure File Operations in Secure Coding Guide.

## See Also

### Related Documentation

func checkResourceIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

### Determining Access to Files

func fileExists(atPath: String, isDirectory: UnsafeMutablePointer&lt;ObjCBool>?) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func isReadableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to read a specified file.

func isWritableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to write to a specified file.

func isExecutableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the operating system appears able to execute a specified file.

func isDeletableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to delete a specified file.

