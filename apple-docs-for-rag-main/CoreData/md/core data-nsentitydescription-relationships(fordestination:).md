

- Core Data
- NSEntityDescription
-  relationships(forDestination:) 

Instance Method

# relationships(forDestination:)

Returns an array containing the relationships of the receiver where the entity description of the relationship is a given entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func relationships(forDestination entity: NSEntityDescription) -> [NSRelationshipDescription]
```

## Parameters 

`entity`  

An entity description.

## Return Value

An array containing the relationships of the receiver where the entity description of the relationship is `entity`. Elements in the array are instances of NSRelationshipDescription.

## See Also

### Working with properties

var propertiesByName: [String : NSPropertyDescription]

A dictionary containing the properties of the receiver.

var properties: [NSPropertyDescription]

An array containing the properties of the receiver.

var attributesByName: [String : NSAttributeDescription]

The attributes of the receiver in a dictionary.

var relationshipsByName: [String : NSRelationshipDescription]

The relationships of the receiver in a dictionary.

