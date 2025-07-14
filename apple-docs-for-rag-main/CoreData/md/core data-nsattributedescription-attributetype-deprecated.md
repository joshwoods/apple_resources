

- Core Data
- NSAttributeDescription
-  attributeType Deprecated

Instance Property

# attributeType

The attribute’s type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var attributeType: NSAttributeType { get set }
```

Deprecated

Use type instead.

## Discussion

Don’t change an attribute’s type after you add its containing managed object model to a persistent store coordinator; otherwise, Core Data throws an exception.

## See Also

### Managing the type

var attributeValueClassName: String?

The class name that represents the attribute’s value.

var type: NSAttributeDescription.AttributeType

The attribute’s type.

struct AttributeType

The types of attributes that Core Data supports.

enum NSAttributeType

The types of attribute that Core Data supports.

