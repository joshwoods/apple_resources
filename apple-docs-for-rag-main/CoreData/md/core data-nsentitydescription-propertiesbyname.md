

- Core Data
- NSEntityDescription
-  propertiesByName 

Instance Property

# propertiesByName

A dictionary containing the properties of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propertiesByName: [String : NSPropertyDescription] { get }
```

## Discussion

The keys in the dictionary are the property names and the values are instances of NSAttributeDescription and/or NSRelationshipDescription.

## See Also

### Working with properties

var properties: [NSPropertyDescription]

An array containing the properties of the receiver.

var attributesByName: [String : NSAttributeDescription]

The attributes of the receiver in a dictionary.

var relationshipsByName: [String : NSRelationshipDescription]

The relationships of the receiver in a dictionary.

func relationships(forDestination: NSEntityDescription) -> [NSRelationshipDescription]

Returns an array containing the relationships of the receiver where the entity description of the relationship is a given entity.

