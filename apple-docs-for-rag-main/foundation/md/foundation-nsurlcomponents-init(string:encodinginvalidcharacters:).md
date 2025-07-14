

- Foundation
- NSURLComponents
-  init(string:encodingInvalidCharacters:) 

Initializer

# init(string:encodingInvalidCharacters:)

Creates a URL components instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init?(
    string URLString: String,
    encodingInvalidCharacters: Bool
)
```

## Parameters 

`URLString`  

The URL string to parse.

`encodingInvalidCharacters`  

A Boolean value that indicates whether the initializer attempts to encode any invalid characters in `URLString`.

## Discussion

If `encodingInvalidCharacters` is `true`, this initializer tries to encode the string to create a valid URL. If the URL string is still invalid after encoding, the initializer returns `nil`.

## See Also

### Creating URL components

init()

Creates a URL components object with all components left undefined.

init?(string: String)

Creates a URL components object by parsing a URL in string form.

init?(url: URL, resolvingAgainstBaseURL: Bool)

Creates a URL components object by parsing the URL from an `NSURL` object.

