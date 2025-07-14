

- Foundation
- NSURLComponents
-  init(url:resolvingAgainstBaseURL:) 

Initializer

# init(url:resolvingAgainstBaseURL:)

Creates a URL components object by parsing the URL from an `NSURL` object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    url: URL,
    resolvingAgainstBaseURL resolve: Bool
)
```

## Parameters 

`url`  

The URL to parse.

`resolve`  

Controls whether the URL should be resolved against its base URL before parsing. If true, and if the `url` parameter contains a relative URL, the original URL is resolved against its base URL before parsing by calling the absoluteURL method. Otherwise, the string portion is used by itself.

## Return Value

Returns the initialized URL components object, or `nil` if the URL could not be parsed.

## See Also

### Creating URL components

init()

Creates a URL components object with all components left undefined.

init?(string: String)

Creates a URL components object by parsing a URL in string form.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

