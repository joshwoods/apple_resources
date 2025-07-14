

- Foundation
- URLProtocol
-  setProperty(\_:forKey:in:) 

Type Method

# setProperty(\_:forKey:in:)

Sets the property associated with the specified key in the specified request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func setProperty(
    _ value: Any,
    forKey key: String,
    in request: NSMutableURLRequest
)
```

## Parameters 

`value`  

The value to set for the specified property.

`key`  

The key for the specified property.

`request`  

The request for which to create the property.

## Discussion

Use this method to provide an interface for protocol implementors to customize protocol-specific information associated with URLRequest objects.

## See Also

### Getting and setting request properties

class func property(forKey: String, in: URLRequest) -> Any?

Fetches the property associated with the specified key in the specified request.

class func removeProperty(forKey: String, in: NSMutableURLRequest)

Removes the property associated with the specified key in the specified request.

