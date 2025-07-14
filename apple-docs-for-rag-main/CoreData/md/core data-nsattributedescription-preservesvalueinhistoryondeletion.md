

- Core Data
- NSAttributeDescription
-  preservesValueInHistoryOnDeletion 

Instance Property

# preservesValueInHistoryOnDeletion

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var preservesValueInHistoryOnDeletion: Bool { get set }
```

## See Also

### Configuring the behavior

var allowsCloudEncryption: Bool

A Boolean value that determines whether to encrypt the attribute’s value.

var allowsExternalBinaryDataStorage: Bool

A Boolean value that indicates whether the attribute allows external binary storage.

var defaultValue: Any?

The default value of the attribute.

var valueTransformerName: String?

The name of the transformer to use for the attribute value.

