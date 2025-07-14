

- Objective-C Runtime
- NSObject
-  inverse(forRelationshipKey:) 

Instance Method

# inverse(forRelationshipKey:)

For a given key that defines the name of the relationship from the receiver’s class to another class, returns the name of the relationship from the other class to the receiver’s class.

Mac CatalystmacOS

``` source
func inverse(forRelationshipKey relationshipKey: String) -> String?
```

## Parameters 

`relationshipKey`  

The name of the relationship from the receiver’s class to another class.

## Return Value

The name of the relationship that is the inverse of the receiver’s relationship named `relationshipKey`.

## Discussion

`NSObject`’s implementation of `inverseForRelationshipKey:` simply invokes `[[self classDescription] inverseForRelationshipKey:relationshipKey]`. To make use of the default implementation, you must therefore implement and register a suitable class description—see NSClassDescription.

For example, suppose an Employee class has a relationship named `department` to a Department class, and that Department has a relationship called `employees` to Employee. The statement:

```
employee inverseForRelationshipKey:@"department"];
```

returns the string `employees`.

## See Also

### Working with Class Descriptions

var attributeKeys: [String]

An array of `NSString` objects containing the names of immutable values that instances of the receiver’s class contain.

var classDescription: NSClassDescription

An object containing information about the attributes and relationships of the receiver’s class.

var toManyRelationshipKeys: [String]

An array containing the keys for the to-many relationship properties of the receiver.

var toOneRelationshipKeys: [String]

The keys for the to-one relationship properties of the receiver, if any.

