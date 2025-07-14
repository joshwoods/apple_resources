

- Core Data
- NSAttributeDescription
-  defaultValue 

Instance Property

# defaultValue

The default value of the attribute.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var defaultValue: Any? { get set }
```

## Discussion

Default values are retained by a managed object model, not copied. This means that attribute values do not have to implement the `NSCopying` protocol, however it also means that you should not modify any objects after they have been set as default values.

### Special Considerations

Setting the default value raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Configuring the behavior

var allowsCloudEncryption: Bool

A Boolean value that determines whether to encrypt the attribute’s value.

var allowsExternalBinaryDataStorage: Bool

A Boolean value that indicates whether the attribute allows external binary storage.

var preservesValueInHistoryOnDeletion: Bool

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

var valueTransformerName: String?

The name of the transformer to use for the attribute value.

