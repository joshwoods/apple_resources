

- Core Data
- NSPropertyDescription
-  isOptional 

Instance Property

# isOptional

A Boolean value that indicates whether the receiver is optional.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isOptional: Bool { get set }
```

## Discussion

true if the receiver is optional, otherwise false. The optionality flag specifies whether a property’s value can be `nil` before an object can be saved to a persistent store.

### Special Considerations

Setting this property raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var name: String

The name of the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

