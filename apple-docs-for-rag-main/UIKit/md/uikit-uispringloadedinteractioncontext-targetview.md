

- UIKit
- UISpringLoadedInteractionContext
-  targetView 

Instance Property

# targetView

The view to which the current spring-loaded interaction view style is applied.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var targetView: UIView? { get set }
```

**Required**

## See Also

### Managing state

var state: UISpringLoadedInteractionEffectState

The current view style for the spring-loaded interaction.

**Required**

var targetItem: Any?

The specific subview, or associated model object, of the target view to use for the spring-loaded interaction.

**Required**

enum UISpringLoadedInteractionEffectState

The spring-loaded interaction states that determine the style of the interaction view.

