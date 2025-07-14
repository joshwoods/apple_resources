

- Swift
- String
-  init(contentsOfFile:usedEncoding:) 

Initializer

# init(contentsOfFile:usedEncoding:)

Produces a string created by reading data from the file at a given path and returns by reference the encoding used to interpret the file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    contentsOfFile path: String,
    usedEncoding: inout String.Encoding
) throws
```

## See Also

### Creating a String from a File or URL

init(contentsOf: URL) throwsDeprecated

init(contentsOf: URL, encoding: String.Encoding) throws

Produces a string created by reading data from a given URL interpreted using a given encoding.

init(contentsOf: URL, usedEncoding: inout String.Encoding) throws

Produces a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

init(contentsOfFile: String) throwsDeprecated

init(contentsOfFile: String, encoding: String.Encoding) throws

Produces a string created by reading data from the file at a given path interpreted using a given encoding.

