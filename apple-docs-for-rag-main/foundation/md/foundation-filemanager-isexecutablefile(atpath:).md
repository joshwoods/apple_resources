

- Foundation
- FileManager
-  isExecutableFile(atPath:) 

Instance Method

# isExecutableFile(atPath:)

Returns a Boolean value that indicates whether the operating system appears able to execute a specified file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isExecutableFile(atPath path: String) -> Bool
```

## Parameters 

`path`  

A file path.

## Return Value

true if the current process has execute privileges for the file at `path`; otherwise false if the process does not have execute privileges or the existence of the file could not be determined.

## Discussion

If the file at `path` is inaccessible to your app, perhaps because it does not have search privileges for one or more parent directories, this method returns false. This method traverses symbolic links in the path. This method also uses the real user ID and group ID, as opposed to the effective user and group IDs, to determine if the file is executable.

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

func isDeletableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to delete a specified file.

