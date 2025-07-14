

- Core Data
- NSPropertyDescription
-  userInfo 

Instance Property

# userInfo

The user info dictionary of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

Setting the user info raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var name: String

The name of the receiver.

