

- Objective-C Runtime
- NSObject
-  attributeKeys 

Instance Property

# attributeKeys

An array of `NSString` objects containing the names of immutable values that instances of the receiver’s class contain.

Mac CatalystmacOS

``` source
var attributeKeys: [String] { get }
```

## Discussion

`NSObject`’s implementation of `attributeKeys` simply calls `[[self classDescription] attributeKeys]`. To make use of the default implementation, you must therefore implement and register a suitable class description—see NSClassDescription.

## See Also

### Working with Class Descriptions

var classDescription: NSClassDescription

An object containing information about the attributes and relationships of the receiver’s class.

func inverse(forRelationshipKey: String) -> String?

For a given key that defines the name of the relationship from the receiver’s class to another class, returns the name of the relationship from the other class to the receiver’s class.

var toManyRelationshipKeys: [String]

An array containing the keys for the to-many relationship properties of the receiver.

var toOneRelationshipKeys: [String]

The keys for the to-one relationship properties of the receiver, if any.

