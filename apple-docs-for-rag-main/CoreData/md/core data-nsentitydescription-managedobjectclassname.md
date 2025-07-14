

- Core Data
- NSEntityDescription
-  managedObjectClassName 

Instance Property

# managedObjectClassName

The name of the class that represents the receiver’s entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var managedObjectClassName: String! { get set }
```

## Discussion

The class specified by `name` must NSManagedObject or a subclass of NSManagedObject.

### Special Considerations

Setting the class name raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Getting descriptive information

var name: String?

The entity name of the receiver.

var managedObjectModel: NSManagedObjectModel

The managed object model with which the receiver is associated.

var renamingIdentifier: String?

The renaming identifier for the receiver.

var isAbstract: Bool

A Boolean value that indicates whether the receiver represents an abstract entity.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

