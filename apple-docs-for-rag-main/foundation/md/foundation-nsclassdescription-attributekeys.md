

- Foundation
- NSClassDescription
-  attributeKeys 

Instance Property

# attributeKeys

Overridden by subclasses to return the names of attributes of instances of the described class.

Mac Catalyst 13.0+macOS 10.0+

``` source
var attributeKeys: [String] { get }
```

## Return Value

An array of `NSString` objects containing the names of attributes of instances of the described class.

## Discussion

For example, a class description that describes Movie objects could return the attribute keys `title`, `dateReleased`, and `rating`.

If you have an instance of the class the receiver describes, you can use the `NSObject` instance method attributeKeys instead.

## See Also

### Related Documentation

var toManyRelationshipKeys: [String]

Overridden by subclasses to return the keys for the to-many relationship properties of instances of the described class.

var toOneRelationshipKeys: [String]

Overridden by subclasses to return the keys for the to-one relationship properties of instances of the described class.

