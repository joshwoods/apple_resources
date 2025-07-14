

- Foundation
- FileManager
-  FileManager.DirectoryEnumerator 

Class

# FileManager.DirectoryEnumerator

An object that enumerates the contents of a directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class DirectoryEnumerator
```

## Overview

You obtain a directory enumerator using FileManager’s enumerator(atPath:) method. The enumeration provides the pathnames of all files and directories contained within that directory. These pathnames are relative to the directory.

An enumeration is recursive, including the files of all subdirectories, and crosses device boundaries. An enumeration does not resolve symbolic links, or attempt to traverse symbolic links that point to directories.

## Topics

### Getting File and Directory Attributes

var directoryAttributes: [FileAttributeKey : Any]?

A dictionary with the attributes of the directory at which enumeration started.

var fileAttributes: [FileAttributeKey : Any]?

A dictionary with the attributes of the most recently returned file or subdirectory (as referenced by the pathname).

var level: Int

The number of levels deep the current object is in the directory hierarchy being enumerated.

### Skipping Subdirectories

func skipDescendents()

Causes the receiver to skip recursion into the most recently obtained subdirectory.

func skipDescendants()

Causes the receiver to skip recursion into the most recently obtained subdirectory.

### Instance Properties

var isEnumeratingDirectoryPostOrder: Bool

## Relationships

### Inherits From

- NSEnumerator

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFastEnumeration
- NSObjectProtocol
- Sequence

## See Also

### Discovering Directory Contents

func contentsOfDirectory(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions) throws -> [URL]

Performs a shallow search of the specified directory and returns URLs for the contained items.

func contentsOfDirectory(atPath: String) throws -> [String]

Performs a shallow search of the specified directory and returns the paths of any contained items.

func enumerator(at: URL, includingPropertiesForKeys: [URLResourceKey]?, options: FileManager.DirectoryEnumerationOptions, errorHandler: ((URL, any Error) -> Bool)?) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified URL.

func enumerator(atPath: String) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified path.

func mountedVolumeURLs(includingResourceValuesForKeys: [URLResourceKey]?, options: FileManager.VolumeEnumerationOptions) -> [URL]?

Returns an array of URLs that identify the mounted volumes available on the device.

struct VolumeEnumerationOptions

Options for enumerating mounted volumes with the mountedVolumeURLs(includingResourceValuesForKeys:options:) method.

func subpathsOfDirectory(atPath: String) throws -> [String]

Performs a deep enumeration of the specified directory and returns the paths of all of the contained subdirectories.

func subpaths(atPath: String) -> [String]?

Returns an array of strings identifying the paths for all items in the specified directory.

