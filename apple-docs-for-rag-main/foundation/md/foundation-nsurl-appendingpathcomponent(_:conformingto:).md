

- Foundation
- NSURL
-  appendingPathComponent(\_:conformingTo:) 

Instance Method

# appendingPathComponent(\_:conformingTo:)

Returns a URL by appending the specified path component with the file extension for a uniform type identifier.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func appendingPathComponent(
    _ partialName: String,
    conformingTo contentType: UTType
) -> URL
```

## Parameters 

`partialName`  

The partial name to append.

`contentType`  

A uniform type identifier the resulting conforms to.

## Return Value

A new URL with the partial name and the type’s preferred extension appended.

## Discussion

Use this method when you want to mix partial input from a user or other source, and need to produce a complete filename suitable for that input. For example, if you download a file from the internet and know its MIME type, you can use this method to ensure the URL has the correct filename extension where you save the file.

If `partialName` already has a path extension, and that path extension is valid for file system objects of type `contentType`, the function doesn’t add an extension before appending it to the URL. For example, if the inputs are `puppy.jpg` and image, respectively, the function returns a URL with an appended path component of `puppy.jpg`. However, if the inputs are `puppy.jpg` and plainText, respectively, the function returns a URL with an appended path component of `puppy.jpg.txt`. If you want to replace any existing path extension, use the deletePathExtension() method first.

If the function can’t append the path component, it returns an unchanged URL.

Note

The modified URL has a directory path if `contentType` conforms to directory.

For more information about types, see Uniform Type Identifiers.

## See Also

### Modifying and Converting a File URL

var filePathURL: URL?

A file path URL that points to the same resource as the URL object. (read-only)

func fileReferenceURL() -> URL?

Returns a new file reference URL that points to the same resource as the receiver.

func appendingPathComponent(String) -> URL?

Returns a new URL by appending a path component to the original URL.

func appendingPathComponent(String, isDirectory: Bool) -> URL?

Returns a new URL by appending a path component to the original URL, along with a trailing slash if the component is a directory.

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

