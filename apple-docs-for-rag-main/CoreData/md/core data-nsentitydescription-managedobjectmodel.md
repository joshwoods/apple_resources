

- Core Data
- NSEntityDescription
-  managedObjectModel 

Instance Property

# managedObjectModel

The managed object model with which the receiver is associated.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var managedObjectModel: NSManagedObjectModel { get }
```

## See Also

### Related Documentation

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

var entities: [NSEntityDescription]

The entities in the model.

### Getting descriptive information

var name: String?

The entity name of the receiver.

var managedObjectClassName: String!

The name of the class that represents the receiver’s entity.

var renamingIdentifier: String?

The renaming identifier for the receiver.

var isAbstract: Bool

A Boolean value that indicates whether the receiver represents an abstract entity.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

