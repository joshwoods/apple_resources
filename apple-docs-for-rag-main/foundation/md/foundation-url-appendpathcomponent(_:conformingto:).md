

- Foundation
- URL
-  appendPathComponent(\_:conformingTo:) 

Instance Method

# appendPathComponent(\_:conformingTo:)

Appends a path component to the URL that conforms to a uniform type identifier.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
mutating func appendPathComponent(
    _ partialName: String,
    conformingTo contentType: UTType
)
```

## Parameters 

`partialName`  

The name of path component without the type.

`contentType`  

A uniform type identifier that determines the default extension.

## Discussion

Use this method when you want to mix partial input from a user or other source, and need to produce a complete filename suitable for that input. For example, if you download a file from the internet and know its MIME type, you can use this method to ensure the URL has the correct filename extension where you save the file.

If `partialName` already has a path extension, and that path extension is valid for file system objects of type `contentType`, the function doesn’t add an extension before appending it to the URL. For example, if the inputs are `puppy.jpg` and jpeg, respectively, the function returns a URL with an appended path component of `puppy.jpg`. However, if the inputs are `puppy.jpg` and plainText, respectively, the function returns a URL with an appended path component of `puppy.jpg.txt`. If you want to replace any existing path extension, use the deletePathExtension() method first.

If the function can’t append the path component, it returns an unchanged URL.

Note

The modified URL has a directory path if `contentType` conforms to directory.

For more information about types, see Uniform Type Identifiers.

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

func append&lt;S>(components: S..., directoryHint: URL.DirectoryHint)

Appends multiple path components to the URL, with a hint for handling directory awareness.

func appending&lt;S>(components: S..., directoryHint: URL.DirectoryHint) -> URL

Returns a new URL by appending multiple path components to the URL, with a hint for handling directory awareness.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component that conforms to a uniform type identifier.

