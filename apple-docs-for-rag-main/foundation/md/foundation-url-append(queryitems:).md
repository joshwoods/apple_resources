

- Foundation
- URL
-  append(queryItems:) 

Instance Method

# append(queryItems:)

Appends a list of query items to the URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func append(queryItems: [URLQueryItem])
```

## Parameters 

`queryItems`  

An array of URLQueryItem instances to append to the URL.

## See Also

### Adding query items

func appending(queryItems: [URLQueryItem]) -> URL

Returns a new URL formed by appending a list of query items to the URL.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

