

- Foundation
- URLRequest
-  setValue(\_:forHTTPHeaderField:) 

Instance Method

# setValue(\_:forHTTPHeaderField:)

Sets a value for the header field.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func setValue(
    _ value: String?,
    forHTTPHeaderField field: String
)
```

## Parameters 

`value`  

The new value for the header field. Any existing value for the field is replaced by the new value.

`field`  

The name of the header field to set. In keeping with the HTTP RFC, HTTP header field names are case insensitive.

## Mentioned in 

Uploading data to a website

## Discussion

Certain header fields are reserved. Do not use this method to set such headers. Specifically, there is no need for you to set the `Content-Length` header. See Reserved HTTP headers.

## See Also

### Accessing header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func value(forHTTPHeaderField: String) -> String?

Retrieves a header value.

