

- Core Data
- NSAttributeDescription
-  allowsCloudEncryption 

Instance Property

# allowsCloudEncryption

A Boolean value that determines whether to encrypt the attribute’s value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var allowsCloudEncryption: Bool { get set }
```

## Mentioned in 

Configuring Attributes

## Discussion

Set this property to true to store the attribute’s value in an encrypted form in iCloud. Only use this property with new attributes. Core Data doesn’t support encrypting attributes that already exist in your CloudKit schema, or attributes that represent relationships between entities.

You can also set this property using the Allow Cloud Encryption attribute in the Attributes inspector of the Core Data model editor.

Important

Attributes can’t change their encryption state after you promote them to your production CloudKit schema. If you choose to encrypt an attribute, it always remains that way.

## See Also

### Configuring the behavior

var allowsExternalBinaryDataStorage: Bool

A Boolean value that indicates whether the attribute allows external binary storage.

var defaultValue: Any?

The default value of the attribute.

var preservesValueInHistoryOnDeletion: Bool

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

var valueTransformerName: String?

The name of the transformer to use for the attribute value.

