

- Core Data
- NSEntityDescription
-  properties 

Instance Property

# properties

An array containing the properties of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var properties: [NSPropertyDescription] { get set }
```

## Discussion

The elements in the array are instances of NSAttributeDescription, NSRelationshipDescription, and/or NSFetchedPropertyDescription.

### Special Considerations

Setting the properties raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Working with properties

var propertiesByName: [String : NSPropertyDescription]

A dictionary containing the properties of the receiver.

var attributesByName: [String : NSAttributeDescription]

The attributes of the receiver in a dictionary.

var relationshipsByName: [String : NSRelationshipDescription]

The relationships of the receiver in a dictionary.

func relationships(forDestination: NSEntityDescription) -> [NSRelationshipDescription]

Returns an array containing the relationships of the receiver where the entity description of the relationship is a given entity.

