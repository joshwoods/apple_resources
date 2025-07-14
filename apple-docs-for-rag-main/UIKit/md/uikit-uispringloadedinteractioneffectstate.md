

- UIKit
-  UISpringLoadedInteractionEffectState 

Enumeration

# UISpringLoadedInteractionEffectState

The spring-loaded interaction states that determine the style of the interaction view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UISpringLoadedInteractionEffectState
```

## Topics

### States

case activated

An interaction state that indicates that the view was spring loaded.

case activating

An interaction state that indicates that spring loading is about to start.

case inactive

An interaction state that indicates that spring loading is not engaged.

case possible

An interaction state that indicates that spring loading is available.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing state

var state: UISpringLoadedInteractionEffectState

The current view style for the spring-loaded interaction.

**Required**

var targetItem: Any?

The specific subview, or associated model object, of the target view to use for the spring-loaded interaction.

**Required**

var targetView: UIView?

The view to which the current spring-loaded interaction view style is applied.

**Required**

