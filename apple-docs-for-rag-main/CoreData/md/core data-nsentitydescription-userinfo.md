

- Core Data
- NSEntityDescription
-  userInfo 

Instance Property

# userInfo

The user info dictionary of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

Setting the user info dictionary raises an exception if the receiver’s model has been used by an object graph manager.

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

var isAbstract: Bool

A Boolean value that indicates whether the receiver represents an abstract entity.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

