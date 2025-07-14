

- UIKit
- UIVisualEffectView
-  init(effect:) 

Initializer

# init(effect:)

Creates a new visual effect view with the designated visual effect.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(effect: UIVisualEffect?)
```

## Parameters 

`effect`  

The UIVisualEffect you provide for the view. This can be a UIBlurEffect or a UIVibrancyEffect.

## Return Value

The new view containing the designated visual effect.

## See Also

### Creating a visual effect view

init?(coder: NSCoder)

Creates a visual effect view from data in an unarchiver.

