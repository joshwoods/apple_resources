

- Foundation
- URL
-  appending(path:directoryHint:) 

Instance Method

# appending(path:directoryHint:)

Returns a URL by appending the specified path to the URL, with a hint for handling directory awareness.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func appending(
    path: S,
    directoryHint: URL.DirectoryHint = .inferFromPath
) -> URL where S : StringProtocol
```

## Parameters 

`path`  

The path to add.

`directoryHint`  

A hint to the method to indicate whether the path is a directory, or to instruct the method to make this determination. Defaults to URL.DirectoryHint.inferFromPath.

## Return Value

A new URL that appends the specified path to the original URL.

## Mentioned in 

Improving performance and stability when accessing the file system

## Discussion

This method doesn’t percent-encode any path separators (`/`) in the path component before appending the component to the path. If you want this encoding, use appending(component:directoryHint:) instead.

## See Also

### Adding path components

func append&lt;S>(path: S, directoryHint: URL.DirectoryHint)

Appends a path to the URL, with a hint for handling directory awareness.

func append&lt;S>(component: S, directoryHint: URL.DirectoryHint)

Appends a path component to the URL, with a hint for handling directory awareness.

func appendPathComponent(String)

Appends a path component to the URL.

Deprecated

func appendPathComponent(String, isDirectory: Bool)

Appends a path component to the URL, specifying whether the resulting path is a directory.

Deprecated

func appending&lt;S>(component: S, directoryHint: URL.DirectoryHint) -> URL

Returns a URL by appending the specified path component to the URL, with a hint for handling directory awareness.

func appendingPathComponent(String) -> URL

Returns a URL by appending the specified path component to self.

Deprecated

func appendingPathComponent(String, isDirectory: Bool) -> URL

Returns a URL by appending the specified path component to self, specifying whether the resulting path is a directory.

Deprecated

func append&lt;S>(components: S..., directoryHint: URL.DirectoryHint)

Appends multiple path components to the URL, with a hint for handling directory awareness.

func appending&lt;S>(components: S..., directoryHint: URL.DirectoryHint) -> URL

Returns a new URL by appending multiple path components to the URL, with a hint for handling directory awareness.

func appendPathComponent(String, conformingTo: UTType)

Appends a path component to the URL that conforms to a uniform type identifier.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component that conforms to a uniform type identifier.

