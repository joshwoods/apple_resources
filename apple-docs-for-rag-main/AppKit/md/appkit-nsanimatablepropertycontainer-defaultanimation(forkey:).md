

- AppKit
- NSAnimatablePropertyContainer
-  defaultAnimation(forKey:) 

Type Method

# defaultAnimation(forKey:)

Returns the default animation that should be performed for the specified key.

macOS 10.5+

``` source
static func defaultAnimation(forKey key: NSAnimatablePropertyKey) -> Any?
```

**Required**

## Parameters 

`key`  

The action name or property specified as a string.

## Return Value

The animation to perform. A subclass of CAAnimation.

## Discussion

The NSAnimatablePropertyContainer method consults this class method when its search of the receivers Getting the Animator Proxy dictionary fails to return an animation for `key`.

An animatable property container should implement this method to return a default animation to be performed for each key that it wants to make auto-animatable, where `key` usually references a property of the receiver, but can also specify a special animation trigger (NSAnimationTriggerOrderIn or NSAnimationTriggerOrderOut).

A developer implementing a custom view subclass, can enable automatic animation for properties by overriding this method, and having it return the desired default CAAnimation subclass to use for each of the property keys of interest. The override should defer to super for any keys it doesn’t specifically handle, facilitating inheritance of default animation specifications. The following is an example of such an implementation.

```
```

## See Also

### Managing Animations for Properties

var animations: [NSAnimatablePropertyKey : Any]

Sets the option dictionary that maps event trigger keys to animation objects.

**Required**

func animation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the animation that should be performed for the specified key.

**Required**

typealias NSAnimatablePropertyKey

