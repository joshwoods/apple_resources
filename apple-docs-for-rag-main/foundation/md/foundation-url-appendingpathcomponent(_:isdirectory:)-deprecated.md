

- Foundation
- URL
-  appendingPathComponent(\_:isDirectory:) Deprecated

Instance Method

# appendingPathComponent(\_:isDirectory:)

Returns a URL by appending the specified path component to self, specifying whether the resulting path is a directory.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func appendingPathComponent(
    _ pathComponent: String,
    isDirectory: Bool
) -> URL
```

Deprecated

Use appending(path:directoryHint:) instead

## Parameters 

`pathComponent`  

The path component to add.

`isDirectory`  

If `true`, the method treats the path component as a directory.

## Return Value

A new URL with the path component appended.

## Discussion

The URL syntax for a directory and for a file at otherwise the same location are slightly different — directory URLs must end in `/`. If you append the path component `second` to the URL `http://www.example.com/first/`, if `isDirectory` is `true`, the resulting URL is `http://www.example.com/first/second/.` If `isDirectory` is `false`, the resulting URL is `http://www.example.com/first/second`.

This difference is particularly important if you resolve another URL against this new URL. For example, the path component `file.html` relative to `http://www.example.com/first/second` is `http://www.apple.com/first/file.html`, whereas relative to `http://www.example.com/first/second/`, it’s `http://www.example.com/first/second/file.html`.

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

func appendingPathComponent(String) -> URL

Returns a URL by appending the specified path component to self.

Deprecated

func append&lt;S>(components: S..., directoryHint: URL.DirectoryHint)

Appends multiple path components to the URL, with a hint for handling directory awareness.

func appending&lt;S>(components: S..., directoryHint: URL.DirectoryHint) -> URL

Returns a new URL by appending multiple path components to the URL, with a hint for handling directory awareness.

func appendPathComponent(String, conformingTo: UTType)

Appends a path component to the URL that conforms to a uniform type identifier.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component that conforms to a uniform type identifier.

