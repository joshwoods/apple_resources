

- AVKit
- AVExperienceController
- AVExperienceController.Experience
-  AVExperienceController.Experience.expanded 

Case

# AVExperienceController.Experience.expanded

An experience where the system places the video outside of its original container.

visionOS 2.0+

``` source
case expanded
```

## Discussion

Transition to this experience to get the appropriate expanded experience for the platform.

It’s valid to transition to this experience even when the original container isn’t in a view hierarchy. In this case, you must specify a fallbackPlacement or the transition result is AVExperienceController.TransitionContext.TransitionResult.reversed(reason:).

Note

This experience to is analogous to a player view controller’s fullscreen state.

## See Also

### Supported experiences

case embedded

An experience where the video embeds within its original container.

case multiview

An experience where multiple videos play together.

