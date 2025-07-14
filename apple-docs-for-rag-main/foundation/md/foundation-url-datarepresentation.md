

- Foundation
- URL
-  dataRepresentation 

Instance Property

# dataRepresentation

The data representation of the URL’s relativeString.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dataRepresentation: Data { get }
```

## Discussion

If the URL was initialized with `init?(dataRepresentation:relativeTo:isAbsolute:)`, the data representation returned are the same bytes as those used at initialization; otherwise, the data representation returned are the bytes of the `relativeString` encoded with UTF8 string encoding.

## See Also

### Working with the data representation of a URL

init?(dataRepresentation: Data, relativeTo: URL?, isAbsolute: Bool)

Initializes a newly created URL using the contents of the given data, relative to a base URL.

