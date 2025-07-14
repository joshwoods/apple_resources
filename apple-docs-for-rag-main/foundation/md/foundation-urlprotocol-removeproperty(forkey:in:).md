

- Foundation
- URLProtocol
-  removeProperty(forKey:in:) 

Type Method

# removeProperty(forKey:in:)

Removes the property associated with the specified key in the specified request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func removeProperty(
    forKey key: String,
    in request: NSMutableURLRequest
)
```

## Parameters 

`key`  

The key whose value should be removed.

`request`  

The request from which to remove the property value.

## Discussion

This method is used to provide an interface for protocol implementors to customize protocol-specific information associated with URLRequest objects, or NSMutableURLRequest objects in Objective-C.

## See Also

### Getting and setting request properties

class func property(forKey: String, in: URLRequest) -> Any?

Fetches the property associated with the specified key in the specified request.

class func setProperty(Any, forKey: String, in: NSMutableURLRequest)

Sets the property associated with the specified key in the specified request.

