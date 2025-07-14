

- Core Data
- NSEntityDescription
-  isAbstract 

Instance Property

# isAbstract

A Boolean value that indicates whether the receiver represents an abstract entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isAbstract: Bool { get set }
```

## Return Value

true if the receiver represents an abstract entity, otherwise false.

## Discussion

true if the receiver represents an abstract entity, otherwise false. An abstract entity might be Shape, with concrete sub-entities such as Rectangle, Triangle, and Circle.

### Special Considerations

Setting whether an entity is abstract raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Getting descriptive information

var name: String?

The entity name of the receiver.

var managedObjectModel: NSManagedObjectModel

The managed object model with which the receiver is associated.

var managedObjectClassName: String!

The name of the class that represents the receiver’s entity.

var renamingIdentifier: String?

The renaming identifier for the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

