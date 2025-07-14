

- Core Data
- NSEntityDescription
-  coreSpotlightDisplayNameExpression 

Instance Property

# coreSpotlightDisplayNameExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var coreSpotlightDisplayNameExpression: NSExpression { get set }
```

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

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

