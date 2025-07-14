

- Foundation
- URL
-  appendingPathComponent(\_:) Deprecated

Instance Method

# appendingPathComponent(\_:)

Returns a URL by appending the specified path component to self.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func appendingPathComponent(_ pathComponent: String) -> URL
```

Deprecated

Use appending(path:directoryHint:) instead

## Parameters 

`pathComponent`  

The path component to add.

## Discussion

For file URLs, this method may perform file system I/O to determine if the path component is a directory, and, if so, it appends a trailing slash `/`. Use appendingPathComponent(_:isDirectory:) if you know the component’s file system object type in advance.

New code should use appending(path:directoryHint:) instead of this method.

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

