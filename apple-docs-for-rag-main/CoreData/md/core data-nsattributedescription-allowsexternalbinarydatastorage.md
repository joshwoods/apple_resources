

- Core Data
- NSAttributeDescription
-  allowsExternalBinaryDataStorage 

Instance Property

# allowsExternalBinaryDataStorage

A Boolean value that indicates whether the attribute allows external binary storage.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var allowsExternalBinaryDataStorage: Bool { get set }
```

## Discussion

true if the attribute allows external binary storage, otherwise false. If this value is true, the corresponding attribute may be stored in a file external to the persistent store itself.

## See Also

### Configuring the behavior

var allowsCloudEncryption: Bool

A Boolean value that determines whether to encrypt the attribute’s value.

var defaultValue: Any?

The default value of the attribute.

var preservesValueInHistoryOnDeletion: Bool

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

var valueTransformerName: String?

The name of the transformer to use for the attribute value.

