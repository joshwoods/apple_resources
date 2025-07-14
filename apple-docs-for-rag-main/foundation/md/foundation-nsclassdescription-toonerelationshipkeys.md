

- Foundation
- NSClassDescription
-  toOneRelationshipKeys 

Instance Property

# toOneRelationshipKeys

Overridden by subclasses to return the keys for the to-one relationship properties of instances of the described class.

Mac Catalyst 13.0+macOS 10.0+

``` source
var toOneRelationshipKeys: [String] { get }
```

## Return Value

An array of `NSString` objects containing the names of the to-one relationship properties of instances of the described class.

## Discussion

To-one relationship properties are single objects.

If you have an instance of the class the receiver describes, you can use the `NSObject` instance method toOneRelationshipKeys instead.

## See Also

### Related Documentation

var attributeKeys: [String]

Overridden by subclasses to return the names of attributes of instances of the described class.

### Relationship keys

func inverse(forRelationshipKey: String) -> String?

Overridden by subclasses to return the name of the inverse relationship from a relationship specified by a given key.

var toManyRelationshipKeys: [String]

Overridden by subclasses to return the keys for the to-many relationship properties of instances of the described class.

