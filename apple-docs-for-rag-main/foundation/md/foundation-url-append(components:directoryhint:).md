

- Foundation
- URL
-  append(components:directoryHint:) 

Instance Method

# append(components:directoryHint:)

Appends multiple path components to the URL, with a hint for handling directory awareness.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func append(
    components: S...,
    directoryHint: URL.DirectoryHint = .inferFromPath
) where S : StringProtocol
```

## Parameters 

`components`  

The path components to add, as a variadic parameter.

`directoryHint`  

A hint to the initializer to indicate whether the path is a directory, or to instruct the method to make this determination. Defaults to URL.DirectoryHint.inferFromPath.

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

func appending&lt;S>(path: S, directoryHint: URL.DirectoryHint) -> URL

Returns a URL by appending the specified path to the URL, with a hint for handling directory awareness.

func appending&lt;S>(component: S, directoryHint: URL.DirectoryHint) -> URL

Returns a URL by appending the specified path component to the URL, with a hint for handling directory awareness.

func appendingPathComponent(String) -> URL

Returns a URL by appending the specified path component to self.

Deprecated

func appendingPathComponent(String, isDirectory: Bool) -> URL

Returns a URL by appending the specified path component to self, specifying whether the resulting path is a directory.

Deprecated

func appending&lt;S>(components: S..., directoryHint: URL.DirectoryHint) -> URL

Returns a new URL by appending multiple path components to the URL, with a hint for handling directory awareness.

func appendPathComponent(String, conformingTo: UTType)

Appends a path component to the URL that conforms to a uniform type identifier.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component that conforms to a uniform type identifier.

