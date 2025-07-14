

- Foundation
- FileManager
-  contentsOfDirectory(atPath:) 

Instance Method

# contentsOfDirectory(atPath:)

Performs a shallow search of the specified directory and returns the paths of any contained items.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contentsOfDirectory(atPath path: String) throws -> [String]
```

## Parameters 

`path`  

The path to the directory whose contents you want to enumerate.

## Return Value

An array of NSString objects, each of which identifies a file, directory, or symbolic link contained in `path`. Returns an empty array if the directory exists but has no contents. In Objective-C, if an error occurs, this method returns `nil` and assigns an appropriate error object to the `error` parameter.

## Discussion

This method performs a shallow search of the directory and therefore does not traverse symbolic links or return the contents of any subdirectories. This method also does not return URLs for the current directory (”`.`”), parent directory (”`..`”), or resource forks (files that begin with “`._`”) but it does return other hidden files (files that begin with a period character). If you need to perform a deep enumeration, use the enumeratorAtURL:includingPropertiesForKeys:options:errorHandler: method instead.

The order of the files in the returned array is undefined.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func fileExists(atPath: String, isDirectory: UnsafeMutablePointer&lt;ObjCBool>?) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

var currentDirectoryPath: String

The path to the program’s current directory.

### Discovering Directory Contents

func contentsOfDirectory(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions) throws -> [URL]

Performs a shallow search of the specified directory and returns URLs for the contained items.

func enumerator(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions, errorHandler: ((URL, any Error) -> Bool)?) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified URL.

func enumerator(atPath: String) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified path.

class DirectoryEnumerator

An object that enumerates the contents of a directory.

func mountedVolumeURLs(includingResourceValuesForKeys: [URLResourceKey]?, options: FileManager.VolumeEnumerationOptions) -> [URL]?

Returns an array of URLs that identify the mounted volumes available on the device.

struct VolumeEnumerationOptions

Options for enumerating mounted volumes with the mountedVolumeURLs(includingResourceValuesForKeys:options:) method.

func subpathsOfDirectory(atPath: String) throws -> [String]

Performs a deep enumeration of the specified directory and returns the paths of all of the contained subdirectories.

func subpaths(atPath: String) -> [String]?

Returns an array of strings identifying the paths for all items in the specified directory.

