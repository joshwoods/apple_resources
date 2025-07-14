

- Swift
- String
-  init(contentsOfFile:) Deprecated

Initializer

# init(contentsOfFile:)

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 8.0–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0+watchOS 2.0–11.0Deprecated

``` source
init(contentsOfFile path: String) throws
```

Deprecated

Use \`init(contentsOfFile:encoding:)\` instead

## See Also

### Creating a String from a File or URL

init(contentsOf: URL) throwsDeprecated

init(contentsOf: URL, encoding: String.Encoding) throws

Produces a string created by reading data from a given URL interpreted using a given encoding.

init(contentsOf: URL, usedEncoding: inout String.Encoding) throws

Produces a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

init(contentsOfFile: String, encoding: String.Encoding) throws

Produces a string created by reading data from the file at a given path interpreted using a given encoding.

init(contentsOfFile: String, usedEncoding: inout String.Encoding) throws

Produces a string created by reading data from the file at a given path and returns by reference the encoding used to interpret the file.

