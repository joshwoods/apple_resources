

- Foundation
- NSURLComponents
-  init() 

Initializer

# init()

Creates a URL components object with all components left undefined.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## Return Value

Returns the initialized URL components object, or `nil` if an error occurs.

## See Also

### Creating URL components

init?(string: String)

Creates a URL components object by parsing a URL in string form.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(url: URL, resolvingAgainstBaseURL: Bool)

Creates a URL components object by parsing the URL from an `NSURL` object.

