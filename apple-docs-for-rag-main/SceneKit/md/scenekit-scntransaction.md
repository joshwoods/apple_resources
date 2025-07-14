

- SceneKit
-  SCNTransaction 

Class

# SCNTransaction

A mechanism for creating implicit animations and combining scene graph changes into atomic updates.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNTransaction
```

## Mentioned in 

Animating SceneKit Content

## Overview

You use SCNTransaction class methods to control the animation that results from changing animatable properties in the scene graph and to combine sets of changes into nested transactions.

### Adding Animation with Automatic Transaction

SceneKit creates a transaction automatically whenever you modify the objects in a scene graph. This transaction groups any additional changes you make from the same thread during the current iteration of that thread’s run loop. When the run loop next iterates, SceneKit automatically commits the transaction, atomically applying all changes made during the transaction to the presentation scene graph (that is, the, version of the scene graph currently being displayed).

Because an automatic transaction has a default duration of zero, any changes it contains appear instantly when SceneKit automatically commits the transaction. By using the `setAnimationDuration(_:)` method in Swift, `setAnimationDuration:` in Objective-C, to change the duration, you *implicitly animate* all changes made to animatable properties during the transaction. You can use implicit animation to add animation to a scene quickly and easily. For example, the code in Listing 1 fades out and moves one node, fades in another, moves and zooms the point of view camera, and focuses a spotlight, all in a single one-second animation.

Listing 1. Implicitly animating several property changes

```
[SCNTransaction setAnimationDuration:1.0];    
_textNode.position = SCNVector3Make(0.0, -10.0, 0.0);
_textNode.opacity = 0.0;
_heroNode.opacity = 1.0;
view.pointOfView = _heroCamera;
_heroCamera.camera.yFov = 20.0;
_lightNode.light.spotInnerAngle = 30.0;
```

### Creating Advanced Animations with Custom Transactions

You can also use SCNTransaction class methods to create and manage a hierarchy of your own transactions. By nesting custom transactions, you can group sets of scene graph changes, applying different animation parameters to each group. Use the begin() method to create a custom transaction, nested within the current transaction if one exists. Use the commit() method to end a transaction, applying all scene graph changes made within.

## Topics

### Creating and Committing Transactions

class func begin()

Begins a new transaction for the current thread.

class func commit()

Commits all changes made during the current transaction.

class func flush()

Applies all changes from the current automatic transaction.

### Overriding Animation Duration and Timing

class var animationDuration: CFTimeInterval

Returns the duration, in seconds, of all animations within the current transaction.

class var animationTimingFunction: CAMediaTimingFunction?

Returns the timing function that SceneKit uses for all animations within this transaction group.

### Temporarily Disabling Property Animations

class var disableActions: Bool

Returns a Boolean value indicating whether changes to animatable properties during the transaction are implicitly animated.

### Getting and Setting Completion Block Objects

class var completionBlock: (() -> Void)?

Returns the block previously associated with the current transaction.

### Managing Concurrency

class func lock()

Attempts to acquire a recursive spinlock to ensure the validity of values you retrieve during the transaction.

class func unlock()

Relinquishes a previously acquired transaction lock.

### Getting and Setting Transaction Properties

class func setValue(Any?, forKey: String)

Associates an arbitrary object with the current transaction using the specified key.

class func value(forKey: String) -> Any?

Returns the object previously associated with the current transaction using the specified key.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

