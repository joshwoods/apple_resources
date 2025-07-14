

- Foundation
- FileManager
-  enumerator(atPath:) 

Instance Method

# enumerator(atPath:)

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerator(atPath path: String) -> FileManager.DirectoryEnumerator?
```

## Parameters 

`path`  

The path of the directory to enumerate.

## Return Value

A FileManager.DirectoryEnumerator object that enumerates the contents of the directory at `path`.

## Discussion

If `path` is a filename, the method returns an enumerator object that enumerates no files—the first call to nextObject() will return `nil`.

Because the enumeration is deep—that is, it lists the contents of all subdirectories—this enumerator object is useful for performing actions that involve large file-system subtrees. This method does not resolve symbolic links encountered in the traversal process, nor does it recurse through them if they point to a directory.

This code fragment enumerates the subdirectories and files under a user’s `Documents` directory and processes all files with an extension of `.doc`:

```
NSString *docsDir = [NSHomeDirectory() stringByAppendingPathComponent:  @"Documents"];
NSFileManager *localFileManager=[[NSFileManager alloc] init];
NSDirectoryEnumerator *dirEnum =
    [localFileManager enumeratorAtPath:docsDir];

NSString *file;
while ((file = [dirEnum nextObject])) {
    if ([[file pathExtension] isEqualToString: @"doc"]) {
        // process the document
        [self scanDocument: [docsDir stringByAppendingPathComponent:file]];
    }
}
```

The FileManager.DirectoryEnumerator class has methods for obtaining the attributes of the existing path and of the parent directory and for skipping descendants of the existing path.

## See Also

### Related Documentation

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

var currentDirectoryPath: String

The path to the program’s current directory.

### Discovering Directory Contents

func contentsOfDirectory(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions) throws -> [URL]

Performs a shallow search of the specified directory and returns URLs for the contained items.

func contentsOfDirectory(atPath: String) throws -> [String]

Performs a shallow search of the specified directory and returns the paths of any contained items.

func enumerator(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions, errorHandler: ((URL, any Error) -> Bool)?) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified URL.

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

