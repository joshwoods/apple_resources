

- Core Animation
-  CATransaction 

Class

# CATransaction

A mechanism for grouping multiple layer-tree operations into atomic updates to the render tree.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CATransaction
```

## Overview

`CATransaction` is the Core Animation mechanism for batching multiple layer-tree operations into atomic updates to the render tree. Every modification to a layer tree must be part of a transaction. Nested transactions are supported.

Core Animation supports two types of transactions: *implicit* transactions and *explicit* transactions. Implicit transactions are created automatically when the layer tree is modified by a thread without an active transaction and are committed automatically when the thread’s runloop next iterates. Explicit transactions occur when the the application sends the CATransaction class a begin() message before modifying the layer tree, and a commit() message afterwards.

CATransaction allows you to override default animation properties that are set for animatable properties. You can customize duration, timing function, whether changes to properties trigger animations, and provide a handler that informs you when all animations from the transaction group are completed.

During a transaction you can temporarily acquire a recursive spin lock for managing property atomicity.

CATransaction supports nested transactions. The following code shows how you can fade out a layer (named `transitioningLayer`) over a 2 second duration while scaling it to three times its original size. The scale animation is within a nested transaction with its own duration of 1 second. After the outer transaction completes, a completion block removes `transitioningLayer` from its parent layer.

```
let transitioningLayer = CALayer()

// Outer transaction animates `opacity` to 0 over 2 seconds
CATransaction.begin()
CATransaction.setAnimationDuration(2)
CATransaction.setCompletionBlock {
    transitioningLayer.removeFromSuperlayer()
}

transitioningLayer.opacity = 0

// Inner transaction animates scale to (3, 3, 3) over 1 second
CATransaction.begin()
CATransaction.setAnimationDuration(1)

transitioningLayer.transform = CATransform3DMakeScale(3, 3, 3)

CATransaction.commit() // Commits inner transaction
CATransaction.commit() // Commits outer transaction
```

## Topics

### Creating and Committing Transactions

class func begin()

Begin a new transaction for the current thread.

class func commit()

Commit all changes made during the current transaction.

class func flush()

Flushes any extant implicit transaction.

### Overriding Animation Duration and Timing

class func animationDuration() -> CFTimeInterval

Returns the animation duration used by all animations within this transaction group.

class func setAnimationDuration(CFTimeInterval)

Sets the animation duration used by all animations within this transaction group.

class func animationTimingFunction() -> CAMediaTimingFunction?

Returns the timing function used for all animations within this transaction group.

class func setAnimationTimingFunction(CAMediaTimingFunction?)

Sets the timing function used for all animations within this transaction group.

### Temporarily Disabling Property Animations

class func disableActions() -> Bool

Returns whether actions triggered as a result of property changes made within this transaction group are suppressed.

class func setDisableActions(Bool)

Sets whether actions triggered as a result of property changes made within this transaction group are suppressed.

### Getting and Setting Completion Block Objects

class func completionBlock() -> (() -> Void)?

Returns the completion block object.

class func setCompletionBlock((() -> Void)?)

Sets the completion block object.

### Managing Concurrency

class func lock()

Attempts to acquire a recursive spin-lock lock, ensuring that returned layer values are valid until unlocked.

class func unlock()

Relinquishes a previously acquired transaction lock.

### Getting and Setting Transaction Properties

class func setValue(Any?, forKey: String)

Sets the arbitrary keyed-data for the specified key.

class func value(forKey: String) -> Any?

Returns the arbitrary keyed-data specified by the given key.

### Constants

Transaction properties

These constants define the property keys used by value(forKey:) and setValue(_:forKey:).

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

## See Also

### Animation Groups

class CAAnimationGroup

An object that allows multiple animations to be grouped and run concurrently.

