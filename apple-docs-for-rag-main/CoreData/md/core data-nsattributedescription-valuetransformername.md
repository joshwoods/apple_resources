

- Core Data
- NSAttributeDescription
-  valueTransformerName 

Instance Property

# valueTransformerName

The name of the transformer to use for the attribute value.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var valueTransformerName: String? { get set }
```

## Discussion

The attribute must be of type `NSTransformedAttributeType`.

The transformer must output an `NSData` object from transformedValue(_:) and must allow reverse transformations.

If this value is `nil`, Core Data uses a default a transformer that uses NSCoding to archive and unarchive the attribute value.

## See Also

### Configuring the behavior

var allowsCloudEncryption: Bool

A Boolean value that determines whether to encrypt the attribute’s value.

var allowsExternalBinaryDataStorage: Bool

A Boolean value that indicates whether the attribute allows external binary storage.

var defaultValue: Any?

The default value of the attribute.

var preservesValueInHistoryOnDeletion: Bool

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

