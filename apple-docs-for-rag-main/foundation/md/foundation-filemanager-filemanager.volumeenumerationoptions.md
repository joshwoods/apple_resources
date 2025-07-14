

- Foundation
- FileManager
-  FileManager.VolumeEnumerationOptions 

Structure

# FileManager.VolumeEnumerationOptions

Options for enumerating mounted volumes with the mountedVolumeURLs(includingResourceValuesForKeys:options:) method.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct VolumeEnumerationOptions
```

## Topics

### Creating a Volume Enumeration Options Value

init(rawValue: UInt)

### Volume Enumeration Options

static var skipHiddenVolumes: FileManager.VolumeEnumerationOptions

The enumeration skips hidden volumes.

static var produceFileReferenceURLs: FileManager.VolumeEnumerationOptions

The enumeration produces file reference URLs rather than path-based URLs.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

class DirectoryEnumerator

An object that enumerates the contents of a directory.

func mountedVolumeURLs(includingResourceValuesForKeys: [URLResourceKey]?, options: FileManager.VolumeEnumerationOptions) -> [URL]?

Returns an array of URLs that identify the mounted volumes available on the device.

func subpathsOfDirectory(atPath: String) throws -> [String]

Performs a deep enumeration of the specified directory and returns the paths of all of the contained subdirectories.

func subpaths(atPath: String) -> [String]?

Returns an array of strings identifying the paths for all items in the specified directory.

