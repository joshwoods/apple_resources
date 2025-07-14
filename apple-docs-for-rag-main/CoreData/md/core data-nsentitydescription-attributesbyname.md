

- Core Data
- NSEntityDescription
-  attributesByName 

Instance Property

# attributesByName

The attributes of the receiver in a dictionary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var attributesByName: [String : NSAttributeDescription] { get }
```

## Discussion

The keys in the dictionary are the attribute names and the values are instances of NSAttributeDescription. .

## See Also

### Working with properties

var propertiesByName: [String : NSPropertyDescription]

A dictionary containing the properties of the receiver.

var properties: [NSPropertyDescription]

An array containing the properties of the receiver.

var relationshipsByName: [String : NSRelationshipDescription]

The relationships of the receiver in a dictionary.

func relationships(forDestination: NSEntityDescription) -> [NSRelationshipDescription]

Returns an array containing the relationships of the receiver where the entity description of the relationship is a given entity.

