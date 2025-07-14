

- Foundation
- FileManager
-  isDeletableFile(atPath:) 

Instance Method

# isDeletableFile(atPath:)

Returns a Boolean value that indicates whether the invoking object appears able to delete a specified file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDeletableFile(atPath path: String) -> Bool
```

## Parameters 

`path`  

A file path.

## Return Value

true if the current process has delete privileges for the file at `path`; otherwise false if the process does not have delete privileges or the existence of the file could not be determined.

## Discussion

For a directory or file to be deletable, the current process must either be able to write to the parent directory of `path` or it must have the same owner as the item at `path`. If `path` is a directory, every item contained in `path` must be deletable by the current process.

If the file at `path` is inaccessible to your app, perhaps because it does not have search privileges for one or more parent directories, this method returns false. If the item at `path` is a symbolic link, it is not traversed.

Note

Attempting to predicate behavior based on the current state of the file system or a particular file on the file system is not recommended. Doing so can cause odd behavior or race conditions. It’s far better to attempt an operation (such as loading a file or creating a directory), check for errors, and handle those errors gracefully than it is to try to figure out ahead of time whether the operation will succeed. For more information on file system race conditions, see Race Conditions and Secure File Operations in Secure Coding Guide.

## See Also

### Determining Access to Files

func fileExists(atPath: String) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func fileExists(atPath: String, isDirectory: UnsafeMutablePointer&lt;ObjCBool>?) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func isReadableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to read a specified file.

func isWritableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to write to a specified file.

func isExecutableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the operating system appears able to execute a specified file.

