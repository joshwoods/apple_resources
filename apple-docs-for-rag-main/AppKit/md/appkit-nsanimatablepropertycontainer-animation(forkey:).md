

- AppKit
- NSAnimatablePropertyContainer
-  animation(forKey:) 

Instance Method

# animation(forKey:)

Returns the animation that should be performed for the specified key.

macOS 10.5+

``` source
func animation(forKey key: NSAnimatablePropertyKey) -> Any?
```

**Required**

## Parameters 

`key`  

The action name or property specified as a string.

## Return Value

The animation to perform. A subclass of CAAnimation.

## Discussion

When the action specified by `key` is triggered for an object, this method is consulted to find the animation, if any, that should be performed in response.

Like its Core Animation CALayer counterpart, action(forKey:), this method is a funnel point that defines the order in which the search for an animation proceeds.It first checks the receiver’s Getting the Animator Proxy dictionary for a value matching `key`, then falls back to animator() for the receiver’s class.

Subclasses should not typically need to override this method.

## See Also

### Related Documentation

func animator() -> Self

Returns a proxy object for the receiver that can be used to initiate implied animation for property changes.

**Required**

### Managing Animations for Properties

var animations: [NSAnimatablePropertyKey : Any]

Sets the option dictionary that maps event trigger keys to animation objects.

**Required**

static func defaultAnimation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the default animation that should be performed for the specified key.

**Required**

typealias NSAnimatablePropertyKey

