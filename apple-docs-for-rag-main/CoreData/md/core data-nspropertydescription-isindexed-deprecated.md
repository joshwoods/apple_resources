

- Core Data
- NSPropertyDescription
-  isIndexed Deprecated

Instance Property

# isIndexed

A Boolean value that indicates whether the receiver should be indexed for searching.

iOS 3.0–11.0DeprecatediPadOS 3.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
var isIndexed: Bool { get set }
```

Deprecated

Use NSEntityDescription.indexes instead

## Discussion

true if the receiver should be indexed for searching, otherwise false. Object stores can optionally use this information upon store creation for operations such as defining indexes.

### Special Considerations

Setting this property raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var name: String

The name of the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

