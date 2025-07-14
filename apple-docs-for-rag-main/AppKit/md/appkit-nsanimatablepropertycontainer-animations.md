

- AppKit
- NSAnimatablePropertyContainer
-  animations 

Instance Property

# animations

Sets the option dictionary that maps event trigger keys to animation objects.

macOS 10.5+

``` source
var animations: [NSAnimatablePropertyKey : Any] { get set }
```

**Required**

## Parameters 

`dict`  

A dictionary containing the event trigger keys and associated animation objects.

## See Also

### Related Documentation

func animator() -> Self

Returns a proxy object for the receiver that can be used to initiate implied animation for property changes.

**Required**

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

### Managing Animations for Properties

func animation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the animation that should be performed for the specified key.

**Required**

static func defaultAnimation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the default animation that should be performed for the specified key.

**Required**

typealias NSAnimatablePropertyKey

