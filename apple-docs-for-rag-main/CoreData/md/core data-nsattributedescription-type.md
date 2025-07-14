

- Core Data
- NSAttributeDescription
-  type 

Instance Property

# type

The attribute’s type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var type: NSAttributeDescription.AttributeType { get set }
```

## Discussion

Don’t change an attribute’s type after you add its containing managed object model to a persistent store coordinator; otherwise, Core Data throws an exception.

## See Also

### Managing the type

var attributeValueClassName: String?

The class name that represents the attribute’s value.

struct AttributeType

The types of attributes that Core Data supports.

var attributeType: NSAttributeType

The attribute’s type.

Deprecated

enum NSAttributeType

The types of attribute that Core Data supports.

