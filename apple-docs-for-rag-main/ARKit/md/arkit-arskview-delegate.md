

- ARKit
- ARSKView
-  delegate 

Instance Property

# delegate

An object you provide to mediate synchronization of the view’s AR scene information with SpriteKit content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
weak var delegate: (any ARSKViewDelegate)? { get set }
```

## See Also

### Responding to AR Updates

protocol ARSKViewDelegate

Methods you can implement to mediate the automatic synchronization of SpriteKit content with an AR session.

