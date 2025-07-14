

- UIKit
- UIDragAnimating
-  addCompletion(\_:) 

Instance Method

# addCompletion(\_:)

Adds an animation completion block to run when a view animation has ended.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addCompletion(_ completion: @escaping (UIViewAnimatingPosition) -> Void)
```

**Required**

## Parameters 

`completion`  

A block that sets animatable view properties.

## See Also

### Adding animations

func addAnimations(() -> Void)

Adds an animation block for modifying a view animation while it’s running.

**Required**

