

- Core Data
- NSEntityDescription
-  renamingIdentifier 

Instance Property

# renamingIdentifier

The renaming identifier for the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var renamingIdentifier: String? { get set }
```

## Discussion

The renaming identifier is used to resolve naming conflicts between models. When creating a mapping model between two managed object models, a source entity and a destination entity that share the same identifier indicate that an entity mapping should be configured to migrate from the source to the destination.

If you do not set this value, the identifier will return the entity’s name.

## See Also

### Getting descriptive information

var name: String?

The entity name of the receiver.

var managedObjectModel: NSManagedObjectModel

The managed object model with which the receiver is associated.

var managedObjectClassName: String!

The name of the class that represents the receiver’s entity.

var isAbstract: Bool

A Boolean value that indicates whether the receiver represents an abstract entity.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

