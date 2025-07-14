

- Core Data
- NSRelationshipDescription
-  inverseRelationship 

Instance Property

# inverseRelationship

The relationship that represents the inverse of the current relationship.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var inverseRelationship: NSRelationshipDescription? { get set }
```

## Discussion

The inverse relationship is the description of the current relationship from the destination entity’s perspective. For example, the inverse of a department’s relationship to an employee (a to-many relationship) is the employees’ relationship to the department (a to-one relationship).

## See Also

### Configuring the Destination

var destinationEntity: NSEntityDescription?

The type of object the relationship contains.

var isOrdered: Bool

A Boolean value that determines whether the relationship preserves the order of the referenced managed objects.

