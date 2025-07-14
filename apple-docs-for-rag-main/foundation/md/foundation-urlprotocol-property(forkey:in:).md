

- Foundation
- URLProtocol
-  property(forKey:in:) 

Type Method

# property(forKey:in:)

Fetches the property associated with the specified key in the specified request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func property(
    forKey key: String,
    in request: URLRequest
) -> Any?
```

## Parameters 

`key`  

The key of the desired property.

`request`  

The request whose properties are to be queried.

## Return Value

The property associated with `key`, or `nil` if no property has been stored for `key`.

## Discussion

Use this method to access protocol-specific information associated with URLRequest objects.

## See Also

### Getting and setting request properties

class func setProperty(Any, forKey: String, in: NSMutableURLRequest)

Sets the property associated with the specified key in the specified request.

class func removeProperty(forKey: String, in: NSMutableURLRequest)

Removes the property associated with the specified key in the specified request.

