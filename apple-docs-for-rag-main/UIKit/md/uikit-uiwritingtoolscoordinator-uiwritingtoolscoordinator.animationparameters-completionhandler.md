

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.AnimationParameters
-  completionHandler 

Instance Property

# completionHandler

A custom block to run when the system animations finish.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
var completionHandler: (() -> Void)? { get set }
```

## Discussion

Set this property to a block that you want the system to run when any animations finish. The block you provide must have no return value and no parameters. The system executes this block once when the current animation finish.

## See Also

### Creating custom animations

var progressHandler: ((Float) -> Void)?

A custom block that runs at the same time as the system animations.

