

- Foundation
- URLComponents
-  init(url:resolvingAgainstBaseURL:) 

Initializer

# init(url:resolvingAgainstBaseURL:)

Creates a URL components instance from a URL string, optionally resolving against a base URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    url: URL,
    resolvingAgainstBaseURL resolve: Bool
)
```

## Parameters 

`url`  

The URL string to parse.

`resolve`  

Controls whether the initializer resolves the URL against its base URL before parsing. If `url` is a relative URL, setting `resolve` to `true` creates components using the absoluteURL property.

## See Also

### Creating URL components

init()

Creates a URL components instance without defining any of the components.

init?(string: String)

Creates a URL components instance from a URL string.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

