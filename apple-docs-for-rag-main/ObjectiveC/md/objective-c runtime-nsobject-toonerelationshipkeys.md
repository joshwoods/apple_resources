

- Objective-C Runtime
- NSObject
-  toOneRelationshipKeys 

Instance Property

# toOneRelationshipKeys

The keys for the to-one relationship properties of the receiver, if any.

Mac CatalystmacOS

``` source
var toOneRelationshipKeys: [String] { get }
```

## See Also

### Working with Class Descriptions

var attributeKeys: [String]

An array of `NSString` objects containing the names of immutable values that instances of the receiver’s class contain.

var classDescription: NSClassDescription

An object containing information about the attributes and relationships of the receiver’s class.

func inverse(forRelationshipKey: String) -> String?

For a given key that defines the name of the relationship from the receiver’s class to another class, returns the name of the relationship from the other class to the receiver’s class.

var toManyRelationshipKeys: [String]

An array containing the keys for the to-many relationship properties of the receiver.

