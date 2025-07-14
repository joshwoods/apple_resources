

- AppKit
-  NSAnimatablePropertyKey 

Type Alias

# NSAnimatablePropertyKey

macOS

``` source
typealias NSAnimatablePropertyKey = String
```

## See Also

### Managing Animations for Properties

var animations: [NSAnimatablePropertyKey : Any]

Sets the option dictionary that maps event trigger keys to animation objects.

**Required**

func animation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the animation that should be performed for the specified key.

**Required**

static func defaultAnimation(forKey: NSAnimatablePropertyKey) -> Any?

Returns the default animation that should be performed for the specified key.

**Required**

