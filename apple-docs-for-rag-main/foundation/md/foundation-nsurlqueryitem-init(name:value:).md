

- Foundation
- NSURLQueryItem
-  init(name:value:) 

Initializer

# init(name:value:)

Initializes a newly allocated query item with the specified name and value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    name: String,
    value: String?
)
```

## Parameters 

`name`  

The name of the query item. For example, in the URL `http://www.apple.com/search/?q=iPad`, the `name` parameter is `q`.

`value`  

The value for the query item. For example, in the URL `http://www.apple.com/search/?q=iPad`, the `value` parameter is `iPad`.

## Return Value

An initialized query item object.

## Discussion

To use the newly initialized query item in composing a URL, add it to the queryItems array of an NSURLComponents instance. Because assigning an array of query items to an NSURLComponents instance automatically encodes the name and value properties, you should not percent-encode these strings.

