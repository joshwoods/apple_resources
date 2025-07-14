

- Foundation
- NSURLQueryItem
-  value 

Instance Property

# value

The value for the query item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var value: String? { get }
```

## Discussion

For example, in the URL `http://www.apple.com/search/?q=iPad`, the `value` parameter is `iPad`.

This string is not percent-encoded.

## See Also

### Related Documentation

var queryItems: [URLQueryItem]?

The query URL component as an array of name/value pairs.

### Reading a Query Item’s Name and Value

var name: String

The name of the query item.

