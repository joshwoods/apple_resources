

- UIKit
-  UISceneActivationConditions 

Class

# UISceneActivationConditions

The set of conditions that define when UIKit activates the current scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UISceneActivationConditions
```

## Overview

When an event occurs that requires the activation of a scene, UIKit routes the event to the scene best suited to handle it. UIKit determines which scene is the best by evaluating the target content identifier of the event against the predicates in each scene’s UISceneActivationConditions object. You create UISceneActivationConditions objects for your scenes and use them to prioritize which events each scene handles. Use the prefersToActivateForTargetContentIdentifierPredicate predicate to designate the scene as the primary handler of an event.

Many different objects contain a targetContentIdentifier property, including NSUserActivity, UNNotificationContent, and UIApplicationShortcutItem. When creating those objects, fill that property with a value that uniquely describes the event and matches your scenes’ predicates. Every event must match at least one scene.

## Topics

### Creating an activation conditions object

init()

Creates a new activation conditions object.

init?(coder: NSCoder)

Restores an activation conditions object from the specified archive.

### Specifying the conditions

var prefersToActivateForTargetContentIdentifierPredicate: NSPredicate

The set of conditions for which UIKit chooses to activate this scene over others.

var canActivateForTargetContentIdentifierPredicate: NSPredicate

Conditions for which UIKit can activate the scene if a better alternative doesn’t exist.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Activation and destruction

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

