

- Foundation
- URL
-  appendPathExtension(for:) 

Instance Method

# appendPathExtension(for:)

Appends the preferred path extension for the type you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
mutating func appendPathExtension(for contentType: UTType)
```

## Parameters 

`contentType`  

A uniform type identifier.

## Discussion

Use this method when you want to mix partial input from a user or other source, and need to produce a complete filename suitable for that input. For example, if you download a file from the internet and know its MIME type, you can use this method to ensure the URL has the correct filename extension where you save the file.

If `partialName` already has a path extension, and that path extension is valid for file system objects of type `contentType`, the function doesn’t add an extension before appending it to the URL. For example, if the inputs are `puppy.jpg` and jpeg, respectively, the function returns a URL with an appended path component of `puppy.jpg`. However, if the inputs are `puppy.jpg` and plainText, respectively, the function returns a URL with an appended path component of `puppy.jpg.txt`. If you want to replace any existing path extension, use the deletePathExtension() method first.

If the function can’t append the path component, it returns an unchanged URL.

For more information about types, see Uniform Type Identifiers.

## See Also

### Adding a path extension

func appendPathExtension(String)

Appends the specified path extension to self.

func appendingPathExtension(String) -> URL

Returns a URL by appending the specified path extension to self.

func appendingPathExtension(for: UTType) -> URL

Returns a URL by appending the preferred path extension for the type you specify to the URL’s last path component.

