

- Foundation
- NSURL
-  fileReferenceURL() 

Instance Method

# fileReferenceURL()

Returns a new file reference URL that points to the same resource as the receiver.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fileReferenceURL() -> URL?
```

## Return Value

The new file reference URL.

## Discussion

File reference URLs use a URL path syntax that identifies a file system object by reference, not by path. This form of file URL remains valid when the file system path of the URL’s underlying resource changes.

If the original URL is a file path URL, this property contains a copy of the URL converted into a file reference URL. If the original URL is a file reference URL, this property contains the original. If the original URL is not a file URL, this property contains `nil`.

File reference URLs cannot be created to file system objects which do not exist or are not reachable. This property contains `nil` instead.

In some areas of the file system hierarchy, file reference URLs cannot be generated to the leaf node of the URL path.

Important

A file reference URL’s path should never be persistently stored, because it is not valid across system restarts or remounts of volumes. If you need to store a persistent reference to a file system object, use a bookmark instead. You can create a bookmark by calling bookmarkData(options:includingResourceValuesForKeys:relativeTo:).

## See Also

### Modifying and Converting a File URL

var filePathURL: URL?

A file path URL that points to the same resource as the URL object. (read-only)

func appendingPathComponent(String) -> URL?

Returns a new URL by appending a path component to the original URL.

func appendingPathComponent(String, isDirectory: Bool) -> URL?

Returns a new URL by appending a path component to the original URL, along with a trailing slash if the component is a directory.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component with the file extension for a uniform type identifier.

func appendingPathExtension(String) -> URL?

Returns a new URL by appending a path extension to the original URL.

func appendingPathExtension(for: UTType) -> URL

Returns a URL by appending the path extension for a uniform type identifier.

var deletingLastPathComponent: URL?

A URL you create by removing the last path component from the receiver. (read-only)

var deletingPathExtension: URL?

A URL you create by removing the path extension from the receiver, if any. (read-only)

var resolvingSymlinksInPath: URL?

A URL that points to the same resource as the receiver and includes no symbolic links. (read-only)

var standardizingPath: URL?

A URL that points to the same resource as the original URL using an absolute path. (read-only)

var hasDirectoryPath: Bool

A Boolean value that indicates whether the URL string’s path represents a directory.

