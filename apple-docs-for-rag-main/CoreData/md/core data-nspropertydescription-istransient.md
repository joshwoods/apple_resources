

- Core Data
- NSPropertyDescription
-  isTransient 

Instance Property

# isTransient

A Boolean value that indicates whether the receiver is transient.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isTransient: Bool { get set }
```

## Discussion

true if the receiver is transient, otherwise false. The transient flag specifies whether or not a property’s value is ignored when an object is saved to a persistent store. Transient properties are not saved to the persistent store, but are still managed for undo, redo, validation, and so on.

### Special Considerations

Setting this property raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var name: String

The name of the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

