

- Foundation
- URLComponents
-  init(string:) 

Initializer

# init(string:)

Creates a URL components instance from a URL string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(string: String)
```

## Parameters 

`string`  

A URL location.

## Discussion

If `string` represents a malformed URL, this initializer returns `nil`.

## See Also

### Creating URL components

init()

Creates a URL components instance without defining any of the components.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(url: URL, resolvingAgainstBaseURL: Bool)

Creates a URL components instance from a URL string, optionally resolving against a base URL.

