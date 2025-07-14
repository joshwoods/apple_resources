

- Foundation
- FileManager
-  fileExists(atPath:isDirectory:) 

Instance Method

# fileExists(atPath:isDirectory:)

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fileExists(
    atPath path: String,
    isDirectory: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`path`  

The path of a file or directory. If `path` begins with a tilde (`~`), it must first be expanded with expandingTildeInPath, or this method will return false.

`isDirectory`  

Upon return, contains true if `path` is a directory or if the final path element is a symbolic link that points to a directory; otherwise, contains false. If `path` doesn’t exist, this value is undefined upon return. Pass `NULL` if you do not need this information.

## Return Value

true if a file at the specified path exists, or false if the file’s does not exist or its existence could not be determined.

## Discussion

If the file at `path` is inaccessible to your app, perhaps because one or more parent directories are inaccessible, this method returns false. If the final element in `path` specifies a symbolic link, this method traverses the link and returns true or false based on the existence of the file at the link destination.

If you need to further determine whether `path` is a package, use the isFilePackage(atPath:) method of NSWorkspace.

doc:#Listing-1 gets an array that identifies the fonts in the user’s fonts directory:

```
NSArray *subpaths;
BOOL isDir;

NSArray *paths = NSSearchPathForDirectoriesInDomains
                     (NSLibraryDirectory, NSUserDomainMask, YES);

if ([paths count] == 1) {

    NSFileManager *fileManager = [[NSFileManager alloc] init];
    NSString *fontPath = [[paths objectAtIndex:0] stringByAppendingPathComponent:@"Fonts"];

    if ([fileManager fileExistsAtPath:fontPath isDirectory:&isDir] && isDir) {
        subpaths = [fileManager subpathsAtPath:fontPath];
// ...
```

Note

Attempting to predicate behavior based on the current state of the file system or a particular file on the file system is not recommended. Doing so can cause odd behavior or race conditions. It’s far better to attempt an operation (such as loading a file or creating a directory), check for errors, and handle those errors gracefully than it is to try to figure out ahead of time whether the operation will succeed. For more information on file-system race conditions, see Race Conditions and Secure File Operations in Secure Coding Guide.

## See Also

### Related Documentation

func checkResourceIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

### Determining Access to Files

func fileExists(atPath: String) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func isReadableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to read a specified file.

func isWritableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to write to a specified file.

func isExecutableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the operating system appears able to execute a specified file.

func isDeletableFile(atPath: String) -> Bool

Returns a Boolean value that indicates whether the invoking object appears able to delete a specified file.

