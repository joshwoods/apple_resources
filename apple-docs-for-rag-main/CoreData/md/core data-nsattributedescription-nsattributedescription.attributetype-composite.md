

- Core Data
- NSAttributeDescription
- NSAttributeDescription.AttributeType
-  composite 

Type Property

# composite

An attribute that derives its value by composing other attributes.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static let composite: NSAttributeDescription.AttributeType
```

## Discussion

Composite attributes support all attribute types except the following:

- undefined

- objectID

- binaryData (when allowsExternalBinaryDataStorage is true)

For more information, see NSCompositeAttributeDescription.

## See Also

### Attribute Types

static let binaryData: NSAttributeDescription.AttributeType

An attribute that stores binary data.

static let boolean: NSAttributeDescription.AttributeType

An attribute that stores a Boolean value.

static let date: NSAttributeDescription.AttributeType

An attribute that stores a date.

static let decimal: NSAttributeDescription.AttributeType

An attribute that stores a decimal value.

static let double: NSAttributeDescription.AttributeType

An attribute that stores a double value.

static let float: NSAttributeDescription.AttributeType

An attribute that stores a float value.

static let integer16: NSAttributeDescription.AttributeType

An attribute that stores a 16-bit signed integer value.

static let integer32: NSAttributeDescription.AttributeType

An attribute that stores a 32-bit signed integer value.

static let integer64: NSAttributeDescription.AttributeType

An attribute that stores a 64-bit signed integer value.

static let objectID: NSAttributeDescription.AttributeType

An attribute that stores a managed object’s ID.

static let string: NSAttributeDescription.AttributeType

An attribute that stores a string.

static let transformable: NSAttributeDescription.AttributeType

An attribute that uses a value transformer to derive its value.

static let undefined: NSAttributeDescription.AttributeType

An attribute that doesn’t have an explicit type.

static let uri: NSAttributeDescription.AttributeType

An attribute that stores a uniform resource identifier.

static let uuid: NSAttributeDescription.AttributeType

An attribute that stores a universally unique identifier.

