

- Foundation
- URL
-  init(dataRepresentation:relativeTo:isAbsolute:) 

Initializer

# init(dataRepresentation:relativeTo:isAbsolute:)

Initializes a newly created URL using the contents of the given data, relative to a base URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    dataRepresentation: Data,
    relativeTo base: URL?,
    isAbsolute: Bool = false
)
```

## Discussion

If the data representation isn’t a legal URL string as ASCII bytes, the URL object may not behave as expected. This initializer returns nil if it can’t form a valid URL from the provided string.

## See Also

### Working with the data representation of a URL

var dataRepresentation: Data

The data representation of the URL’s relativeString.

