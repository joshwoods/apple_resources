

- UIKit
- UIDragAnimating
-  addAnimations(\_:) 

Instance Method

# addAnimations(\_:)

Adds an animation block for modifying a view animation while it’s running.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addAnimations(_ animations: @escaping () -> Void)
```

**Required**

## Parameters 

`animations`  

A block that sets animatable view properties.

## See Also

### Adding animations

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds an animation completion block to run when a view animation has ended.

**Required**

