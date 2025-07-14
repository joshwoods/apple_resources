

- Foundation
- FileManager
-  mountedVolumeURLs(includingResourceValuesForKeys:options:) 

Instance Method

# mountedVolumeURLs(includingResourceValuesForKeys:options:)

Returns an array of URLs that identify the mounted volumes available on the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func mountedVolumeURLs(
    includingResourceValuesForKeys propertyKeys: [URLResourceKey]?,
    options: FileManager.VolumeEnumerationOptions = []
) -> [URL]?
```

## Parameters 

`propertyKeys`  

An array of keys that identify the file properties that you want pre-fetched for each volume. For each returned URL, the values for these keys are cached in the corresponding NSURL objects. You may specify `nil` for this parameter. For a list of keys you can specify, see Common File System Resource Keys.

`options`  

Option flags for the enumeration. For a list of possible values, see FileManager.VolumeEnumerationOptions.

## Return Value

An array of `NSURL` objects identifying the mounted volumes.

Important

This method returns `nil` on platforms other than macOS.

## Discussion

This call may block if I/O is required to determine values for the requested `propertyKeys`.

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

struct VolumeEnumerationOptions

Options for enumerating mounted volumes with the mountedVolumeURLs(includingResourceValuesForKeys:options:) method.

func subpathsOfDirectory(atPath: String) throws -> [String]

Performs a deep enumeration of the specified directory and returns the paths of all of the contained subdirectories.

func subpaths(atPath: String) -> [String]?

Returns an array of strings identifying the paths for all items in the specified directory.

